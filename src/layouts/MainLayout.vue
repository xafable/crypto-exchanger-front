<template>
  <q-layout view="hHh lpR fFf">


    <q-header class="bg-dark text-white" height-hint="98">
      <div class="c-container">
        <div class="row justify-between">
          <div class="col-4">
            <q-img
              :src="'https://i.ibb.co/mR49B6K/Pngtree-simple-logo-vector-3174709.png'"
              spinner-color="white"
              style="height: 40px;width: 480px;margin-bottom: 30px"
            />
          </div>
          <div class="col-6" style="padding-left: 15%">
            <q-btn @click="$router.push('/')"  stretch flat label="Home" />
            <q-btn  stretch flat label="Our coins" />
            <q-btn  stretch flat label="Reviews" />
            <q-btn  stretch flat label="Contact" />

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
            <p class="text-h4 text-white" style="text-align: center">Services</p>


            <q-list dense padding class="rounded-borders">

              <q-item  v-ripple>
                <q-item-section>
                  <q-btn stretch flat label="Home" />
                </q-item-section>
              </q-item>

              <q-item  v-ripple>
                <q-item-section>
                  <q-btn  stretch flat label="Our coins" />
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


            <q-list dense bordered padding class="rounded-borders">

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
                <q-btn icon="fa-brands fa-telegram" color="white" stretch flat label="Telegram: @u-swap" />
            </div>
            <br>
            <div class="row">
              <q-btn icon="email" color="white" stretch flat label="Email: contact@u-swap.com" />
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
</style>
