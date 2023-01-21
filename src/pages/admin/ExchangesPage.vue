<template>
  <div class="c-container">
    <q-markup-table>
      <thead>
      <tr>
        <th class="text-left">ApplicationId</th>
        <th class="text-right">Coin</th>
        <th class="text-right">Amount</th>
        <th class="text-right">Status</th>
      </tr>
      </thead>
      <tbody>
      <tr v-for="item in applications" :key="item.calories">
        <td class="text-left">{{ item.ApplicationId }}</td>
        <td class="text-right">{{ item.fromCoin.title }} -> {{ item.toCoin.title }}</td>
        <td class="text-right">
          <q-badge color="primary">{{ item.fromCoin.amount }}</q-badge> -> {{ item.toCoin.amount }}
        </td>
        <td>
          <q-select
            color="secondary"
            @update:model-value="tes($event,item.ApplicationId)"
            v-model="item.status.description"
            :options="options"
            label="Status" />
        </td>

      </tr>

      </tbody>
    </q-markup-table>
  </div>
</template>

<script>

const rows = [
  {
    name: 'Frozen Yogurt',
    calories: 159,
    fat: 6.0,
    carbs: 24,
  },
  {
    name: 'Ice cream sandwich',
    calories: 237,
    fat: 9.0,
    carbs: 37,
  }]


export default {
  name: "ExchangesPage",
  setup(){
    return {
      rows
    }
  },
  data() {
    return {
      model:[],
      options: [],
      applications: [],
      dataLoaded: false
    }
  },
  methods:{
    tes(it,r){
      console.log(r)
    },
    async loadStatuses(){
      await fetch('https://exapi.vikarecept.com/api/v1/statuses',{
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
              label: item.description,
              value: item.title
            })
          })
          this.options = opt
          this.dataLoaded = true

        })
        .catch( error =>  {
        })
    },
    async loadApplications(){
      await fetch('https://exapi.vikarecept.com/api/v1/application/load',{
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

          this.applications = data.data
          this.dataLoaded = true

        })
        .catch( error =>  {
        })
    },
  },
  created() {
    this.loadStatuses()
    this.loadApplications()
  }
}
</script>

<style scoped>
.c-container {
  width: 80%;
  margin-right: auto;
  margin-left: auto;
}
</style>
