<template>
  <div v-if="dataLoaded">
    <div class="row">
      <div class="col-8" >
        <q-select
          color="secondary"
          v-model="fromCoin.coin" :options="options" label="Coin" />
      </div>
      <div class="col-4">
        <q-input clearable
                 type="number"
                 color="secondary"
          v-model="fromCoin.amount" label="Amount" />
      </div>
    </div>
    <br>
    <q-btn round
           style="margin-left: 50%;"
           @click="onSwap"
           size="20px"
           icon="import_export"
    />
    <br>
    <div class="row">
      <div class="col-8">
        <q-select
          color="secondary"
          v-model="toCoin.coin" :options="options" label="Coin" />
      </div>
      <div class="col-4">
        <q-input
          readonly
          color="secondary"
          type="number"
          v-model="toCoin.amount" label="Amount" />
      </div>
    </div>

    <br><br>
    <p class="text-h5 text-black">Crypto wallet address</p>
    <q-input
      ref="applicantWalletAddress"
      color="secondary"
      v-model="applicantWalletAddress"
      label="wallet address" />
    <br><br>
    <p class="text-h5 text-black">Email for tracking the status of the application (optional)</p>
    <q-input
      color="secondary"
      v-model="applicantEmail" label="email" />

    <br>
    <q-checkbox
      ref='agreeCheckbox'
      color="secondary"
      v-model="agreeCheckbox"
      label="I agree with our Privacy Policy and exchange rules" />

    <br><br>
    <q-btn
      @click="onNext"
      size="15px"
      rounded
      color="secondary"
      label="Next" />

  </div>









</template>

<script>
import { useQuasar } from 'quasar'

export default {
  name: "CryptoExchanger",
  setup() {
    const $q = useQuasar()

    return {
      $q
    }
  },
  data() {
    return{
      fromCoin: {
        coin:'',
        amount:0
      },
      toCoin: {
        coin:'',
        amount:0
      },
      applicantWalletAddress: '',
      applicantEmail: '',
      agreeCheckbox: false,
      model: null,
      options: [],
      dataLoaded: false
    }
  },
  methods: {
    async loadCoins(){
      await fetch('https://exapi.vikarecept.com/api/v1/coins/available',{
        method: 'GET',
        headers: {
          'Accept': 'application/json',
        },
      })
        .then(response => {
          if (response.ok) {
            return response.json();
          }
          else
            return response.json().then(data => { throw new Error(data.message) })
        })
        .then(data => {
          let opt = []
          data.data.forEach(function (item) {
            opt.push({
              label: item.title,
              value: item
            })

          })
          this.options = opt
          this.dataLoaded = true
        })
        .catch( error =>  {
          this.errorNotify()
        })
    },
    async calculatePrice(){
      await fetch('https://exapi.vikarecept.com/api/v1/coins/get?fromCoin='
        +this.fromCoin.coin.value.title+'&toCoin='+this.toCoin.coin.value.title+'&fromAmount='+this.fromCoin.amount,{
        method: 'GET',
        headers: {
          'Accept': 'application/json',
        },
      })
        .then(response => {
          if (response.ok) {
            return response.json();
          }
          else
            return response.json().then(data => { throw new Error(data.message) })
        })
        .then(data => {
          this.toCoin.amount = data.data.amount
        })
        .catch( error =>  {
          this.errorNotify()
        })

    },
    async postApplication(){

      let data = new FormData()
      data.append('fromCoinTitle', this.fromCoin.coin.value.title)
      data.append('toCoinTitle', this.toCoin.coin.value.title)
      data.append('fromCoinAmount', this.fromCoin.amount)
      data.append('applicantWalletAddress', this.applicantWalletAddress)
      data.append('applicantEmail', this.applicantEmail)
      data.append('applicantInfo', 'info')
      data.append('fromBlockchain', this.fromCoin.coin.value.blockchain)
      data.append('toBlockchain', this.toCoin.coin.value.blockchain)



      return await fetch('https://exapi.vikarecept.com/api/v1/application/create',{
        method: 'POST',
        headers: {
          'Accept': 'application/json',
        },
        body: data,
      })
        .then(response => {
          if (response.ok) {
            return response.json();
          }
          else
            return response.json().then(data => { throw new Error(data.message) })
        })
        .then(data => {
          return data.data.ApplicationId
        })
        .catch( error =>  {
          this.errorNotify()
        })
    },
    async onSwap(){
      let temp = this.fromCoin
      this.fromCoin = this.toCoin
      this.toCoin = temp
      this.fromCoin.amount = 0
      this.toCoin.amount = 0
    },
    async onNext() {
      if(this.applicantWalletAddress.length < 1) {
        this.$refs['applicantWalletAddress'].$el.focus()
        this.$q.notify({
          message: 'Wallet Address is Required',
          color: 'indigo'
        })
      }

      if(!this.agreeCheckbox) {
        this.$refs['agreeCheckbox'].$el.focus()
        this.$q.notify({
          message: 'You need to agree with rules',
          color: 'indigo'
        })
      }

      if(this.agreeCheckbox && this.applicantWalletAddress.length > 1) {
        let id = await this.postApplication()
        this.$router.push(`/application/`+id)
      }


    },
    async errorNotify(){
      this.$q.notify({
        message: 'Something wrong. Reload page or try later.',
        color: 'red'
      })
    }
  },
  created() {
    this.loadCoins()
  },
  watch: {
    fromCoin: {
      handler(newValue, oldValue) {
        if(newValue.amount > 0){
          if(newValue.amount < newValue.coin.value.minimalExchange)
            this.$q.notify({
              message: 'Minimal exchange for this coin:  ' + newValue.coin.value.minimalExchange,
              color: 'indigo'
            })
          else
            this.calculatePrice()
        }

      },
      deep: true
    },
    'toCoin.coin': function (newValue, oldValue) {
      if(this.fromCoin.amount > 0)
        this.calculatePrice()
    }
  }
}
</script>

<style scoped>

</style>
