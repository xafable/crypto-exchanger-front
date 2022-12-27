<template>

  <div class="q-pa-md" style="max-width: 350px">
    <q-list style="max-width: 50%">

      <q-item v-for="item in coins" :key="item" clickable v-ripple>
        <q-item-section avatar>
          <q-avatar color="teal" text-color="white" icon="currency_bitcoin" />
        </q-item-section>
        <q-item-section>
          <p class="text-h6">{{ item.title }}</p>
          <p>{{  item.available }}</p>
        </q-item-section>
      </q-item>


    </q-list>
  </div>
</template>

<script>
export default {
  name: "CoinList",
  data() {
    return {
      coins: {},
      dataLoaded: false
    }
  },
  methods: {
    async loadCoins(){
      await fetch('http://exchanger-api/api/v1/coins/available',{
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
          this.coins = data.data
          this.dataLoaded = true
        })
        .catch( error =>  {
          this.$store.dispatch('toastMessage',error.message)
        })
    }
  },
  mounted() {
    this.loadCoins()
  }
}
</script>

<style scoped>

</style>
