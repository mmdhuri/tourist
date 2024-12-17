<template>
  <div class="contact-us-banner">
    <div class="row justify-center q-py-xl">
      <div class="col-xs-10 col-md-4 shadow-2">
        <div class="contact-form q-pa-md">
          <h4 class="text-center">Connect with us</h4>
          <div class="q-gutter-md">
            <q-form class="q-gutter-md">

              <q-input v-model="name" label="Name" stack-label autofocus lazy-rules :dense="dense"
                :rules="[val => val && val.length > 0 || 'Please type something']" />
              <q-input v-model="email" label="Email" stack-label type="email" lazy-rules
                :rules="[val => val && val.length > 0 || 'Please type something']" />
              <q-input v-model="message" label="Message" stack-label type="textarea" rows="5" />
              <q-btn type="submit" label="Submit" color="primary" />
            </q-form>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { ref } from 'vue'

const model = ref({
  name: "",
  email: "",
  message: ""
})
</script>
<style scoped>
.contact-form {
  background: rgba(255, 255, 255, 0.2);
  box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
  backdrop-filter: blur(5.5px);
  -webkit-backdrop-filter: blur(5.5px);
  border-radius: 10px;
  border: 1px solid rgba(255, 255, 255, 0.18);
}
</style>
