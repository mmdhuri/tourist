<template>
  <section class="landing-banner">
    <div class="container">
      <div class="text-right q-py-xl text-white relative-position" style="z-index: 9;">
        <h1 class="q-my-sm font-size-74 text-bold" style="line-height: 3rem;">Welcome to Sindhudurg</h1>
        <p class="text-uppercase font-size-22">Whether you seek adventure, relaxation,
          <br> or cultural enrichment Sindhudurg promises memories to last a lifetime.
        </p>
      </div>
    </div>
  </section>
  <section class="q-pb-xl">
    <div class="container">
      <h2 class="font-size-30 text-weight-medium text-center">Most Popular Tours</h2>

      <div class="q-pa-md">
        <q-carousel v-model="slide" transition-prev="slide-right" transition-next="slide-left" swipeable animated
          control-color="amber" navigation padding arrows height="100%" class="">
          <q-carousel-slide :name="1" class="column no-wrap">
            <div class="row fit justify-start items-center q-gutter-xs q-col-gutter no-wrap">
              <div class="example-item col-md-6 col-lg-3 q-ma-none full-height ">
                <q-card flat bordered class="q-ma-sm no-border no-border-radius full-height">
                  <img src="~src/assets/Site Images/nature/evening-sun.jpg" width="300" style="height: 300px;">
                  <q-card-section>
                    <div class="text-h6">Solitary Bird at Sunset</div>
                    <div class="text-subtitle2">The sky is painted with shades of orange and pink, creating a serene and
                      tranquil moment as the day comes to a close.</div>
                  </q-card-section>
                </q-card>
              </div>
              <div class="example-item col-md-6 col-lg-3 q-ma-none full-height">
                <q-card flat bordered class="q-ma-sm no-border no-border-radius full-height"
                  style="border-radius: 0px;">
                  <img src="~src/assets/Site Images/nature/sea.jpg" width="300" style="height: 300px;">
                  <q-card-section>
                    <div class="text-h6">Rainy Dusk by the Sea</div>
                    <div class="text-subtitle2">The rhythmic sound of the waves adds a calming melody to this tranquil
                      scene,
                      capturing the essence of Goa's rainy season.</div>
                  </q-card-section>
                </q-card>
              </div>
              <div class="example-item col-md-6 col-lg-3 q-ma-none full-height">
                <q-card flat bordered class="q-ma-sm no-border no-border-radius" style="border-radius: 0px;">
                  <img src="~src/assets/Site Images/nature/Nature_Tree.jpeg" width="300" style="height: 300px;">
                  <q-card-section>
                    <div class="text-h6">Tree Base View</div>
                    <div class="text-subtitle2">The image showcases the intricate network of roots spreading outwards,
                      creating a natural tapestry that intertwines with the earth.
                    </div>
                  </q-card-section>
                </q-card>
              </div>
              <div class="example-item col-md-6 col-lg-3 q-ma-none full-height">
                <q-card flat bordered class="q-ma-sm no-border no-border-radius" style="border-radius: 0px;">
                  <img src="~src/assets/Site Images/nature/Rainbow.jpg" width="300" style="height: 300px;">
                  <q-card-section>
                    <div class="text-h6">Rainbow Bliss</div>
                    <div class="text-subtitle2">The spectrum of red, orange, yellow, green, blue, indigo, and violet
                      stretches
                      gracefully, offering a moment of serenity and wonder.</div>
                  </q-card-section>
                </q-card>
              </div>
            </div>
          </q-carousel-slide>
          <q-carousel-slide :name="2" class="column no-wrap">
            <div class="row fit justify-start items-center q-gutter-xs q-col-gutter no-wrap">
              <div class="example-item col-md-6 col-lg-3 q-ma-none full-height">
                <q-card flat bordered class="q-ma-sm no-border no-border-radius full-height"
                  style="border-radius: 0px;">
                  <img src="~src/assets/Site Images/nature/evening-sun.jpg" width="300" style="height: 300px;">
                  <q-card-section>
                    <div class="text-h6">Solitary Bird at Sunset</div>
                    <div class="text-subtitle2">The sky is painted with shades of orange and pink, creating a serene and
                      tranquil moment as the day comes to a close.</div>
                  </q-card-section>
                </q-card>
              </div>
              <div class="example-item col-md-6 col-lg-3 q-ma-none full-height">
                <q-card flat bordered class="q-ma-sm no-border no-border-radius full-height"
                  style="border-radius: 0px;">
                  <img src="~src/assets/Site Images/nature/sea.jpg" width="300" style="height: 300px;">
                  <q-card-section>
                    <div class="text-h6">Rainy Dusk by the Sea</div>
                    <div class="text-subtitle2">The rhythmic sound of the waves adds a calming melody to this tranquil
                      scene,
                      capturing the essence of Goa's rainy season.</div>
                  </q-card-section>
                </q-card>
              </div>
              <div class="example-item col-md-6 col-lg-3 q-ma-none full-height">
                <q-card flat bordered class="q-ma-sm no-border no-border-radius" style="border-radius: 0px;">
                  <img src="~src/assets/Site Images/nature/Nature_Tree.jpeg" width="300" style="height: 300px;">
                  <q-card-section>
                    <div class="text-h6">Tree Base View</div>
                    <div class="text-subtitle2">The image showcases the intricate network of roots spreading outwards,
                      creating a natural tapestry that intertwines with the earth.
                    </div>
                  </q-card-section>
                </q-card>
              </div>
              <div class="example-item col-md-6 col-lg-3 q-ma-none full-height">
                <q-card flat bordered class="q-ma-sm no-border no-border-radius" style="border-radius: 0px;">
                  <img src="~src/assets/Site Images/nature/Rainbow.jpg" width="300" style="height: 300px;">
                  <q-card-section>
                    <div class="text-h6">Rainbow Bliss</div>
                    <div class="text-subtitle2">The spectrum of red, orange, yellow, green, blue, indigo, and violet
                      stretches
                      gracefully, offering a moment of serenity and wonder.</div>
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
    <q-video :ratio="16 / 9" src="https://www.youtube.com/embed/Ctdbz3woWJY?si=qaAyzBOQS-APJGJF" />
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
