<template>
<div>
  <p class="text-h5 text-black">Your name:</p>
  <q-input
    color="secondary"
    v-model="Name" label="Name" />
  <br><br>
  <p class="text-h5 text-black">Your contact (Email, mobile ,telegram etc):</p>
  <q-input
    color="secondary"
    v-model="Contact" label="Contact" />
  <q-btn @click="sendTicket" rounded color="secondary" label="Contact with me"  size="20px" style="margin-top: 40px"/>
</div>
</template>

<script>
import {useQuasar} from "quasar";

export default {
  name: "TicketSend",
  setup() {
    const $q = useQuasar()

    return {
      $q
    }
  },
  data() {
    return {
      name: '',
      contact: ''
    }
  },
  methods: {
    async sendTicket(){
      let data = new FormData()
      data.append('contactName', this.name)
      data.append('contactAddress', this.contact)


      await fetch('https://exapi.vikarecept.com/api/v1/ticket/create',{
        method: 'POST',
        headers: {
          'Accept': 'application/json',
        },
        body: data
      })
        .then(response => {
          if (response.ok) {
            return response.json();
          }
          else
            return response.json().then(data => { throw new Error(data.message) })
        })
        .then(data => {
          this.$q.notify({
            message: 'Sent. We will contact you soon.',
            color: 'indigo'
          })

          this.name = ''
          this.contact = ''
        })
        .catch( error =>  {
          //this.errorNotify()
        })
    }
  }
}

</script>

<style scoped>

</style>
