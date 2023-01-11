<template>
  <q-scroll-area style="height: 350px;">
    <div class="c-container">
      <transition-group name="list" tag="ul">
        <q-list>

          <div v-for="item in applications" :key="item.applicantEmail">
            <q-item >
              <q-item-section>
                <q-item-label class="text-white">{{ item.applicantEmail }}</q-item-label>
                <q-item-label class="text-white" caption lines="2"> {{item.fromCoinTitle }} -> {{item.toCoinTitle}}</q-item-label>
              </q-item-section>
              <q-item-section side top>
                <q-item-label class="text-white" caption> {{ item.fromCoinAmount }} -> {{item.toCoinAmount}}</q-item-label>
              </q-item-section>
            </q-item>
            <q-separator spaced inset />
          </div>

        </q-list>
      </transition-group>
    </div>
  </q-scroll-area>


</template>

<script>
import {useQuasar} from "quasar";

export default {
  name: "LatestExchanges",
  setup() {
    const $q = useQuasar()

    return {
      $q
    }
  },
  data() {
    return {
      applications: [],
      tempApplications: [],
      dataLoaded: false
    }
  },
  methods: {
    async fetchLatestApplications() {
      await fetch('https://exapi.vikarecept.com/api/v1/application/get/last',{
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
          this.applications = data.data.slice(0,20)
          this.tempApplications = data.data.slice(21,100)
          this.dataLoaded = true
        })
        .catch( error =>  {
          this.errorNotify()
        })
    },
    async addApplications(){
      if(this.tempApplications.length > 0) {
        let rand = Math.floor(Math.random() * this.tempApplications.length)
        this.applications.unshift(this.tempApplications[rand])
        this.tempApplications.splice(rand, 1);
      }
      else {
         this.fetchLatestApplications()
      }
    }
  },
  created() {
    this.fetchLatestApplications()
    setInterval(this.addApplications,10000)
  }
}
</script>

<style scoped>
.c-container {
  width: 50%;
  margin-right: auto;
  margin-left: auto;
}
.list-enter-active, .list-leave-active {
  transition: all 1s;
}
.list-enter, .list-leave-to /* .list-leave-active below version 2.1.8 */ {
  opacity: 0;
  transform: translateX(-295px);
}
</style>
