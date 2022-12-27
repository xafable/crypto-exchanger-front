<template>
  <q-page class="">


      <div style="background-color: #1D1D1D;position: relative">
        <div class="c-container">
          <div class="row justify-between" style="padding-top: 50px">
            <transition name="slide" appear>
            <div class="col-4">
              <div class="row" style="padding-top: 30px">
                <p class="text-h1 text-white">Make crypto </p>
              </div>
              <div class="row">
                <p class="text-h1 text-brand">exchanged easily </p>
              </div>
              <div class="row">
                <p class="text-white">Fast processing. Low commissions. Best conditions. </p>
              </div>
              <q-btn rounded color="secondary" label="Change crypto" />
            </div>
            </transition>
            <transition name="slide-2" appear>
            <div class="col-4">
              <img src="https://i.ibb.co/ZWDfRTJ/yyyyy7.png" style="height:100%; "/>
            </div>
            </transition>
          </div>

        </div>
      </div>



    <div style="background-color: #ffffff;">
      <div class="c-container benefits__wrap"  >
        <div class="q-pa-md row q-gutter-md justify-center">

          <q-card dark bordered class="bg-secondary my-card">
            <q-card-section>
              <div class="text-h6">
                Best exchange rate of crypto</div>
            </q-card-section>
            <q-separator dark inset />
            <q-card-section>
              Automated system for processing applications. Tools for controlling status and time of the converting.
            </q-card-section>
          </q-card>

          <q-card dark bordered class="bg-secondary my-card">
            <q-card-section>
              <div class="text-h6">Dynamic crypto market rates</div>
              <div class="text-subtitle2"></div>
            </q-card-section>
            <q-separator dark inset />
            <q-card-section>
              Always the most profitable offer on the market. WiseSwap makes a rate fixation while you filling in the application.
            </q-card-section>
          </q-card>

          <q-card dark bordered class="bg-secondary my-card">
            <q-card-section>
              <div class="text-h6">Protected exchange report</div>
              <div class="text-subtitle2"></div>
            </q-card-section>
            <q-separator dark inset />
            <q-card-section>
              We provide an easy protected application report for our clients. Detailed information in real time.
            </q-card-section>
          </q-card>

          <q-card dark bordered class="bg-secondary my-card">
            <q-card-section>
              <div class="text-h6">U-Swap Support 24/7</div>
              <div class="text-subtitle2"></div>
            </q-card-section>
            <q-separator dark inset />
            <q-card-section>
              Our support service is always ready to help you. Telegram, Email or Contact form is on our website.
            </q-card-section>
          </q-card>

        </div>

      </div>
    </div>



    <div style="background-color: #ffffff;position: relative;margin-top: 200px">
      <div class="c-container">
        <div class="row" style="padding-top: 50px">

            <div class="col-6">
            <div class="row" style="padding-top: 30px">
              <p class="text-h2 text-black">Immediate crypto exchange</p>
            </div>
            <br><br>
            <CryptoExchanger></CryptoExchanger>
            </div>

            <div class="col-6">
              <br>
              <div style="margin-left: 30%">
                <p class="text-h2 text-black">Coin List</p>

                <q-scroll-area style="height: 600px;">
                  <CoinList></CoinList>
                </q-scroll-area>
              </div>

            </div>

        </div>
      </div>
    </div>


    <div style="background-color: #1D1D1D;margin-top: 150px">
      <div class="c-container">
        <FeedbackSlider></FeedbackSlider>

          <div class="column items-center" style="padding-bottom: 100px;">
            <div class="col">
              <FeedbackSend @feedbackSended = "showNotification('Feedback sended')"></FeedbackSend>
            </div>
          </div>
      </div>
    </div>


    <div style="background-color: #ffffff;position: relative;margin-top: 200px">
      <div class="c-container">
        <div class="row" style="padding-top: 50px">

          <div class="col-6">

            <p class="text-h5 text-black">Your name:</p>
            <q-input
              color="secondary"
              v-model="text" label="name" />
            <br><br>
            <p class="text-h5 text-black">Email or mobile:</p>
            <q-input
              color="secondary"
              v-model="text" label="email or mobile" />
            <q-btn rounded color="secondary" label="Contact with me"  size="20px" style="margin-top: 40px"/>

          </div>

          <div class="col-6">
            <div style="margin-left: 20%">
              <p class="text-h5">We are always happy to help our clients!</p>
              <p>Are you left with any questions or faced any troubles while using our service, please let us know!
                Contact our support we will do our best to help you!</p>

              <div class="row">
                <q-btn size="20px" icon="fa-brands fa-telegram" color="black" stretch flat label="Telegram: @u-swap" />
              </div>
              <br>
              <div class="row">
                <q-btn size="20px" icon="email" color="black" stretch flat label="Email: contact@u-swap.com" />
              </div>

            </div>



          </div>

        </div>
      </div>
    </div>



    <br>
    <br>
    <br>
    <br>
    <br>



  </q-page>
</template>

<script>
import { defineComponent } from 'vue'
import { useQuasar } from 'quasar'
import CryptoExchanger from "components/CryptoExchanger.vue"
import CoinList from "components/CoinList.vue"
import FeedbackSlider from "components/FeedbackSlider.vue"
import FeedbackSend from "components/FeedbackSend.vue"





export default defineComponent({
  name: 'IndexPage',
  setup() {
    const $q = useQuasar()

    return {
      $q
    }
  },
  components: {
    CryptoExchanger,
    CoinList,
    FeedbackSlider,
    FeedbackSend,
  },
  methods: {
    showNotification(message){
      this.$q.notify({
        message: message,
        color: 'secondary'
      })
    }
  }
})
</script>
<style scoped>
.c-container {
  width: 80%;
  margin-right: auto;
  margin-left: auto;
}
.text-brand {
  color: #39C9C6 !important;
}
.text-white {
  color: #ffffff !important;
}
.benefits__wrap {
  gap: 24px;
  position: relative;
  z-index: 1;
  margin-top: -94px;
}

</style>

<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 250px

</style>

<style lang="scss" scoped>

.slide-enter {
  opacity: 0;
}
.slide-enter-active {
  animation: slide-in 1s ease-in forwards;
  transition: opacity .5s;
}
.slide-leave {
  // initial state set in keyframe
}
.slide-leave-active {
  animation: slide-out 1s ease-out forwards;
  opacity: 0;
  transition: opacity 1s;
}
@keyframes slide-in {
  from {
    transform: translateX(-1200px);
  }
  to {
    transform: translateX(0);
  }
}
@keyframes slide-out {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(120px);
  }
}

/////
.slide-2-enter {
  opacity: 0;
}
.slide-2-enter-active {
  animation: slide-2-in 1.5s ease-in forwards;
  transition: opacity .5s;
}
.slide-2-leave {
  // initial state set in keyframe
}
.slide-2-leave-active {
  animation: slide-2-out 1s ease-out forwards;
  opacity: 0;
  transition: opacity 1s;
}
@keyframes slide-2-in {
  from {
    transform: translateX(1400px);
  }
  to {
    transform: translateX(0);
  }
}
@keyframes slide-2-out {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(-1020px);
  }
}
</style>
