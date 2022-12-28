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
    <q-btn round style="margin-left: 50%;"
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
      color="secondary"
      v-model="text" label="wallet address" />
    <br><br>
    <p class="text-h5 text-black">Email for tracking the status of the application (optional)</p>
    <q-input
      color="secondary"
      v-model="text" label="email" />
  </div>









</template>

<script>
export default {
  name: "CryptoExchanger",
  data() {
    return{
      fromCoin: {
        coin:'',
        amount:''
      },
      toCoin: {
        coin:'',
        amount:''
      },
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
          //this.options = data.data

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

        })
    },
    async onSwap(){
      let temp = this.fromCoin
      this.fromCoin = this.toCoin
      this.toCoin = temp
      this.fromCoin.amount = ''
      this.toCoin.amount = ''

    }
  },
  created() {
    this.loadCoins()
  },
  watch: {
    fromCoin: {
      handler(newValue, oldValue) {
        alert(newValue)

      },
      deep: true
    }
  }
}
</script>

<style scoped>

</style>
