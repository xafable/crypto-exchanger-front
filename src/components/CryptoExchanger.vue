<template>
  <div>
    <div class="row">
      <div class="col-8" >
        <q-select
          color="secondary"
          v-model="model" :options="options" label="Coin" />
      </div>
      <div class="col-4">
        <q-input
          color="secondary"
          v-model="text" label="Amount" />
      </div>
    </div>
    <br>
    <q-btn round style="margin-left: 50%;"
           size="20px"
           icon="import_export"
    />
    <br>
    <div class="row">
      <div class="col-8">
        <q-select
          color="secondary"
          v-model="model" :options="options" label="Coin" />
      </div>
      <div class="col-4">
        <q-input
          color="secondary"
          v-model="text" label="Amount" />
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
      model: null,
      options: [
        'Google', 'Facebook', 'Twitter', 'Apple', 'Oracle'
      ]
    }
  },
}
</script>

<style scoped>

</style>
