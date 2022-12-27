
  <template>
    <div class="q-pa-md q-gutter-sm">
      <q-btn label="Send feedback" rounded color="secondary" @click="prompt = true" />

      <q-dialog v-model="prompt" persistent>
        <q-card style="width: 60%">
          <q-card-section>
            <div class="text-h6">Name</div>
            <q-input
              aria-required
              color="secondary"
              dense
              v-model="name"
              autofocus
              @keyup.enter="prompt = false" />
          </q-card-section>
          <br>
          <q-card-section class="q-pt-none">
            <div class="text-h6">Feedback</div>
            <q-input
              color="secondary"
              v-model="text"
              filled
              type="textarea"
            />
          </q-card-section>

          <q-card-actions align="right" class="text-primary">
            <q-btn color="secondary" flat label="Cancel" v-close-popup />
            <q-btn @click="onSend" color="secondary" flat label="Send" v-close-popup />
          </q-card-actions>
        </q-card>
      </q-dialog>
    </div>
  </template>


<script>
import { ref } from 'vue'
export default {
 name: "FeedbackSend",
 setup () {
    return {
      prompt: ref(false),
      address: ref('')
    }
  },
  methods: {
   onSend(){
     this.$emit('feedbackSended')
   }
  }
}
</script>

<style scoped>

</style>
