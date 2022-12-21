<template>

  <div class="q-pa-md" style="max-width: 350px">
    <q-list style="max-width: 50%">

      <q-item v-for="item in 50" :key="item" clickable v-ripple>
        <q-item-section avatar>
          <q-avatar color="teal" text-color="white" icon="currency_bitcoin" />
        </q-item-section>
        <q-item-section>
          <p class="text-h6">Bitcoin</p>
          <p>8.9999</p>
        </q-item-section>
      </q-item>


    </q-list>
  </div>
</template>

<script>
export default {
  name: "CoinList"
}
</script>

<style scoped>

</style>
