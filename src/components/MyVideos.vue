<template>
  <div class="">
    <q-video :ratio="16 / 9" src="https://www.youtube.com/embed/jWPTJeTym1Q?si=ViTzSQcaravmhmqA" />
  </div>
  <div class="q-pa-md">
    <div></div>
    <div class="row">
      <div class="col-md-3">
        <q-card class="my-card">
          <q-video :ratio="16 / 9" src="https://www.youtube.com/embed/o3s7R8EUFaI?si=uAoGi-7hpFJE6DZP" />

          <q-card-section>
            <div class="text-h6">श्री देवी माऊली सोनुर्ली🙏 जत्रा🥳 | *लोटांगण* #कोकण #जत्रा</div>
          </q-card-section>

          <q-card-section class="q-pt-none">
            🙏🌺 | लोटांगण जत्रेसाठी प्रसिद्ध असलेले सोनुर्ली येथील श्री देवी माऊली जत्रोत्सव 2024 | 🌺🙏
            #कोकण #जत्रा

            सोनुर्ली देवी माऊली मंदिर सावंतवाडी तालुक्यातील हे मंदिर महामार्गापासून अंदाजे ३ किमी आत आहे. येथील जत्रा
            'लोटांगण जत्रे'साठी प्रसिद्ध आहे, जी दिवाळीनंतर तुळशीविवाहाच्या दुसऱ्या तिसऱ्या दिवशी आयोजित केली जाते.
            मनापासून प्रार्थना केली आणि आभार मानून देवीला लोटांगण घातलं तर तुमची इच्छा पूर्ण होते असा ....
          </q-card-section>
        </q-card>
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
