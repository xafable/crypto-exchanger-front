<template>
  <q-layout view="hHh lpR fFf">


    <q-header class="bg-dark text-white" height-hint="98">
      <div class="c-container">
        <div class="row justify-between">
          <div class="col-4">
            <q-img
              @click="imgClick"
              :src="'https://i.ibb.co/mR49B6K/Pngtree-simple-logo-vector-3174709.png'"
              spinner-color="white"
              style="height: 40px;width: 480px;margin-bottom: 30px"
            />
          </div>
          <div class="col-6" style="padding-left: 15%">
            <q-btn @click="$router.push('/')"  stretch flat label="Home" />
            <q-btn @click="$router.push('/#change')" stretch flat label="Our coins" />
            <q-btn @click="$router.push('/#review')"  stretch flat label="Reviews" />
            <q-btn @click="$router.push('/#contact')"  stretch flat label="Contact" />

          </div>
          <div class="col-2">

            <q-btn  rounded color="secondary" label="Change crypto" />

          </div>
        </div>



      </div>

    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <div class="bg-dark text-white">

      <div class="bg-secondary" style="height: 10px"></div>

      <div class="c-container">


        <div class="row">
          <div class="col-1"></div>
          <div class="col-4">
            <p class="text-h4 text-white">Services</p>


            <q-list dense padding class="rounded-borders">

              <q-item  v-ripple>
                <q-item-section>
                  <q-btn stretch flat label="Home" />
                </q-item-section>
              </q-item>

              <q-item  v-ripple>
                <q-item-section>
                 <q-btn @click="$router.push('/#change')" stretch flat label="Our coins" />
                </q-item-section>
              </q-item>

              <q-item  v-ripple>
                <q-item-section>
                  <q-btn  stretch flat label="Reviews" />
                </q-item-section>
              </q-item>

              <q-item  v-ripple>
                <q-item-section>
                  <q-btn  stretch flat label="Contact" />
                </q-item-section>
              </q-item>
            </q-list>
          </div>
          <div class="col-4">
            <p class="text-h4 text-white" style="text-align: center">Documents</p>


            <q-list dense  padding class="rounded-borders">

              <q-item  v-ripple>
                <q-item-section>
                  <q-btn stretch flat label="Privacy Policy" />
                </q-item-section>
              </q-item>

              <q-item  v-ripple>
                <q-item-section>
                  <q-btn  stretch flat label="Terms of use" />
                </q-item-section>
              </q-item>

              <q-item  v-ripple>
                <q-item-section>
                  <q-btn  stretch flat label="AML/KYC" />
                </q-item-section>
              </q-item>

              <q-item  v-ripple>
                <q-item-section>
                  <q-btn  stretch flat label="Rules" />
                </q-item-section>
              </q-item>
            </q-list>
          </div>
          <div class="col-3">
            <p class="text-h4 text-white" style="text-align: center"> </p>

            <div class="row">
                <q-btn icon="fa-brands fa-telegram" color="white" stretch flat label="Telegram: @unlimited" />
            </div>
            <br>
            <div class="row">
              <q-btn icon="email" color="white" stretch flat label="Email: contact@unlimited.com" />
            </div>
            <br>
            <div class="row bottom-btn">

              <q-btn  rounded color="secondary" label="Change crypto" />

            </div>
            </div>



        </div>



      </div>
      <div class="bg-secondary copyright">
        <div class="cc-container">
          <div class="row justify-between">
            <div class="col-5">
              Copyright © 2017 - {{getCurrentYear()}} - Unlimited | All rights reserved
            </div>
            <div class="col-3">
              Linked to: <a href="https://t.me/" target="_blank" class="t-link"><i class="fab fa-telegram tt-link"></i></a>
            </div>
          </div>
        </div>
      </div>


    </div>



  </q-layout>
</template>

<script>

import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'MainLayout',
  components: {

  },
  setup () {

    const leftDrawerOpen = ref(false)

    return {
      leftDrawerOpen,
      toggleLeftDrawer () {
      leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  },
  methods: {
    imgClick() {
      this.$router.push('/')
    },
    getCurrentYear(){
      return new Date().getFullYear();
    }

  }
})
</script>
<style scoped>
.c-q-tabs {
  /*padding-right: 20%;*/
}
.c-container {
  margin-top: 15px;
  width: 80%;
  margin-right: auto;
  margin-left: auto;
}
.cc-container {
  width: 80%;
  margin-right: auto;
  margin-left: auto;
}

.bottom-btn{
  margin-left: 25%;
}

.copyright{
  padding: 15px;
  /*min-width: 25px;*/
}

.t-link{
  color: inherit;
  text-decoration: none;
}

.tt-link{
  font-size: 15px;
}

</style>
