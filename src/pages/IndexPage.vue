<template>
  <section class="landing-banner">
    <div class="container">
      <div class="text-right q-py-xl text-white relative-position" style="z-index: 9;">
        <h1 class="q-my-md font-size-38 font-size-lg-74 line-height-3 text-bold">Welcome to Sindhudurg</h1>
        <p class="text-uppercase font-size-lg-22 font-size-16">Whether you seek adventure, relaxation,
          <br> or cultural enrichment Sindhudurg promises memories to last a lifetime.
        </p>
      </div>
    </div>
  </section>
  <section class="q-pb-xl">
    <div class="container">
      <h2 class="font-size-30 text-weight-medium text-center">Most Popular Places</h2>
      <div class="row  justify-start items-center ">
        <div class=" col-md-6 col-lg-3 q-ma-none full-height ">
          <q-card flat bordered class="q-ma-sm no-border no-border-radius full-height">
            <img src="~src/assets/Site Images/Populer Places/Bhogve Beach.jpg" width="300" style="height: 300px;">
            <q-card-section>
              <div class="text-h6">Bhogwe Beach</div>
              <div class="text-subtitle3">Bhogave beach is endowed with foamy waves and silver sand. Village Bhogave has
                another attraction of unification of sea and river named Karli. </div>
              <q-btn class="q-mt-sm" color="primary" size="sm" label="Read More" />
            </q-card-section>
          </q-card>
        </div>
        <div class=" col-md-6 col-lg-3 q-ma-none full-height">
          <q-card flat bordered class="q-ma-sm no-border no-border-radius full-height" style="border-radius: 0px;">
            <img src="~src/assets/Site Images/Populer Places/tarkarli_beach.jpeg" width="300" style="height: 300px;">
            <q-card-section>
              <div class="text-h6">Tarkarli Beach</div>
              <div class="text-subtitle3">It is a beach destination and remote place in southern Maharashtra. A few
                years ago, Tarkarli beach was declared a Queen Beach of the Konkan region.</div>
              <q-btn class="q-mt-sm" color="primary" size="sm" label="Read More" />
            </q-card-section>
          </q-card>
        </div>
        <div class="col-md-6 col-lg-3 q-ma-none full-height">
          <q-card flat bordered class="q-ma-sm no-border no-border-radius" style="border-radius: 0px;">
            <img src="~src/assets/Site Images/Populer Places/devbag-sangam-beach.jpeg" width="300"
              style="height: 300px;">
            <q-card-section>
              <div class="text-h6">Devbagh Sangham</div>
              <div class="text-subtitle3">Devbagh is known for its serene and uncrowded beaches, delectable seafood, and
                as an ideal destination for a beach vacation.</div>
              <q-btn class="q-mt-sm" color="primary" size="sm" label="Read More" />

            </q-card-section>
          </q-card>
        </div>
        <div class="col-md-6 col-lg-3 q-ma-none full-height">
          <q-card flat bordered class="q-ma-sm no-border no-border-radius" style="border-radius: 0px;">
            <img src="~src/assets/Site Images/Populer Places/sindhudurg_fort.jpeg" width="300" style="height: 300px;">
            <q-card-section>
              <div class="text-h6">Sindhudurg Fort</div>
              <div class="text-subtitle3">Sindhudurg Fort (Marathi pronunciation: [sin̪d̪ʱud̪uɾɡ]) is a historical sea
                fort located in Arabian Sea near the Konkan region of Maharashtra in Western India.[1] </div>
              <q-btn class="q-mt-sm" color="primary" size="sm" label="Read More" />

            </q-card-section>
          </q-card>
        </div>
      </div>
      <div class="q-pa-md hidden">
        <q-carousel v-model="slide" transition-prev="slide-right" transition-next="slide-left" swipeable animated
          control-color="amber" navigation padding arrows height="100%" class="">
          <q-carousel-slide :name="1" class="column no-wrap">
            <div class="row  justify-start items-center ">
              <div class=" col-md-6 col-lg-3 q-ma-none full-height ">
                <q-card flat bordered class="q-ma-sm no-border no-border-radius full-height">
                  <img src="~src/assets/Site Images/Populer Places/Bhogve Beach.jpg" width="300" style="height: 300px;">
                  <q-card-section>
                    <div class="text-h6">Bhogwe Beach</div>
                    <div class="text-subtitle2"></div>
                  </q-card-section>
                </q-card>
              </div>
              <div class=" col-md-6 col-lg-3 q-ma-none full-height">
                <q-card flat bordered class="q-ma-sm no-border no-border-radius full-height"
                  style="border-radius: 0px;">
                  <img src="~src/assets/Site Images/Populer Places/tarkarli_beach.jpeg" width="300"
                    style="height: 300px;">
                  <q-card-section>
                    <div class="text-h6">Tarkarli Beach</div>
                    <div class="text-subtitle2"></div>
                  </q-card-section>
                </q-card>
              </div>
              <div class="col-md-6 col-lg-3 q-ma-none full-height">
                <q-card flat bordered class="q-ma-sm no-border no-border-radius" style="border-radius: 0px;">
                  <img src="~src/assets/Site Images/Populer Places/devbag-sangam-beach.jpeg" width="300"
                    style="height: 300px;">
                  <q-card-section>
                    <div class="text-h6">Devbag Sangham</div>
                    <div class="text-subtitle2"></div>
                  </q-card-section>
                </q-card>
              </div>
              <div class="col-md-6 col-lg-3 q-ma-none full-height">
                <q-card flat bordered class="q-ma-sm no-border no-border-radius" style="border-radius: 0px;">
                  <img src="~src/assets/Site Images/Populer Places/sindhudurg_fort.jpeg" width="300"
                    style="height: 300px;">
                  <q-card-section>
                    <div class="text-h6">Sindhudurg Fort</div>
                    <div class="text-subtitle2"></div>
                  </q-card-section>
                </q-card>
              </div>
            </div>
          </q-carousel-slide>
        </q-carousel>
      </div>

    </div>
  </section>
  <section class="">

  </section>
</template>

<script setup>
import { ref, onMounted } from 'vue';

const slide = ref(1);

defineOptions({
  name: 'IndexPage'
});
</script>
<style scoped>
.q-card {
  box-shadow: 0px 0px 2px #878787 !important;
}

.example-item>div {
  height: 100% !important;
}
</style>
