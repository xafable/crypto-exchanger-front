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
            <q-btn  stretch flat label="Home" />
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
  padding-right: 20%;
}
.c-container {
  margin-top: 15px;
  width: 80%;
  margin-right: auto;
  margin-left: auto;
}
</style>
