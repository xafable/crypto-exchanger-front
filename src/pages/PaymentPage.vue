<template>

  <div v-if="dataLoaded">


    <div style="background-color: #1D1D1D;position: relative">
      <div class="c-container" style="height: 200px">
        <div class="row justify-between" >



              <div class="text-h2">
                Application
                <span class="text-h2">
                  {{  application.ApplicationId }}
                </span>
              </div>

          <div class="text-h4 bg-secondary wit-btn">Waiting for payment
            <q-icon class="spinner" name="fa-solid fa-spinner" />
          </div>


        </div>

      </div>
    </div>



    <div class="c-container benefits__wrap">
      <div class="q-pa-md row q-gutter-md justify-around">

        <q-card  bordered class="my-card col-3">
          <q-card-section>
            <div class="text-h6">Application ID:</div>
            <q-badge class="bg-secondary" align="middle">{{  application.ApplicationId }}</q-badge>
          </q-card-section>
          <q-separator inset />
          <q-card-section>
            <div class="text-h6">Status:</div>
            <q-badge class="bg-secondary" align="middle">{{ application.status.description }}</q-badge>
          </q-card-section>
          <q-separator inset />
          <q-card-section>
            <div class="text-h6">Date:</div>
            <q-badge class="bg-secondary" align="middle">{{  application.createdAt }}</q-badge>
          </q-card-section>
          <q-separator inset />
          <q-card-section>
            <div class="text-h6">Page link:</div>
            link
          </q-card-section>
        </q-card>

        <q-card  bordered class="my-card col-4">
          <q-card-section>
            <div class="row justify-center">
              <div class="col-5">
                <img src="https://raw.githubusercontent.com/spothq/cryptocurrency-icons/1a63530be6e374711a8554f31b17e4cb92c25fa5/svg/color/eth.svg" style="height:30px; "/>
                {{ application.fromCoin.shortTitle }}
              </div>
              <div class="col-2">
                <q-icon class="sp" name="fa-solid fa-arrow-right" />
              </div>
              <div class="col-5">
                {{ application.toCoin.shortTitle }}
              </div>
            </div>
          </q-card-section>
          <q-separator inset />
          <q-card-section>
            <div>
              <div>Amount: {{ application.toCoin.amount }}  ({{ application.fromCoin.shortTitle }}) to the address:</div>
              <div>{{  application.toCoin.walletAddress }}</div>
              <div>in {{ application.toCoin.blockchain }} Network</div>
            </div>
          </q-card-section>
          <q-separator inset />
          <q-card-section>
            <div>
              <div>Waller for receiving in {{ application.toCoin.shortTitle }}:</div>
              <div>{{ application.fromCoin.walletAddress }}</div>
              <div>in ERC20 Network</div>
            </div>
          </q-card-section>
        </q-card>




        <q-card  bordered class="my-card col-2">
          <q-card-section>
            <div>
              <qrcode-vue value="pidor" size="170" level="H" />
            </div>
          </q-card-section>
          <q-card-section>
            Pay us faster in BTC with QR-code
          </q-card-section>
        </q-card>



      </div>
    </div>



  </div>



</template>

<script>


import QrcodeVue from 'qrcode.vue'


export default {
  name: "PaymentPage",
  components:{
    QrcodeVue
  },
  setup() {

  },
  data () {
    return {
      application: {},
      dataLoaded: false
    }
  },
  methods: {
    async fetchApplication(){

      await fetch('https://exapi.vikarecept.com/api/v1/application/19',{
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
          this.application = data.data
          this.dataLoaded = true
        })
        .catch( error =>  {
          this.$store.dispatch('toastMessage',error.message)
        })
    }
  },
  created() {
    this.fetchApplication()
  }
}
</script>

<style scoped>
.c-container {
  width: 80%;
  margin-right: auto;
  margin-left: auto;
}

.my-card{
  border-radius: 30px;
}

.benefits__wrap {
  gap: 24px;
  position: relative;
  z-index: 1;
  margin-top: -94px;
}

.wit-btn{
  padding: 10px;
  border-radius: 30px;
}


.spinner{
  animation-name: spin;
  animation-duration: 2000ms;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}
@keyframes spin {
  from {
    transform:rotate(0deg);
  }
  to {
    transform:rotate(360deg);
  }
}

</style>
