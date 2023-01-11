<template>
  <div class="c-container">
    <q-markup-table>
      <thead>
      <tr>
        <th class="text-left">Dessert (100g serving)</th>
        <th class="text-right">Calories</th>
        <th class="text-right">Fat (g)</th>
        <th class="text-right">Carbs (g)</th>
      </tr>
      </thead>
      <tbody>
      <tr v-for="item in rows" :key="item.calories">
        <td class="text-left">{{ item.name }}</td>
        <td class="text-right">{{ item.calories }}</td>
        <td class="text-right">{{ item.fat }}</td>
        <td class="text-right">
          <q-select
            @update:model-value="tes($event,22)"
            v-model="model"
            :options="options"
            label="Standard" />
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
      model: '',
      options: [
        'Google', 'Facebook', 'Twitter', 'Apple', 'Oracle'
      ]
    }
  },
  methods:{
    tes(it,r){
      //alert(it)
      console.log(r)
    },
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
          this.errorNotify()
        })
    },

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
