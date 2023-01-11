<template>

<div>
  <q-carousel
    v-model="slide"
    transition-prev="scale"
    transition-next="scale"
    swipeable
    animated
    control-color="white"
    navigation
    padding
    arrows
    height="300px"
    class="bg-dark text-white "
  >

    <q-carousel-slide name="style" class="column no-wrap flex-center">
      <p class="text-h5">Aashit</p>
      <span>4.5                 <q-icon name="grade" size="34px" /></span>
      <div class="q-mt-md text-center">
        {{ lorem }}
      </div>
    </q-carousel-slide>
    <q-carousel-slide name="tv" class="column no-wrap flex-center">
      <q-icon name="grade" size="56px" />
      <div class="q-mt-md text-center">
        {{ lorem }}
      </div>
    </q-carousel-slide>
    <q-carousel-slide name="layers" class="column no-wrap flex-center">
      <q-icon name="grade" size="56px" />
      <div class="q-mt-md text-center">
        {{ lorem }}
      </div>
    </q-carousel-slide>
    <q-carousel-slide name="map" class="column no-wrap flex-center">
      <q-icon name="grade" size="56px" />
      <div class="q-mt-md text-center">
        {{ lorem }}
      </div>
    </q-carousel-slide>

  </q-carousel>
</div>

</template>

<script>
import { ref } from 'vue'

export default {
  name: "FeedbackSlider",
  setup () {
    return {
      slide: ref('style'),
      lorem: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque voluptatem totam, architecto cupiditate officia rerum, error dignissimos praesentium libero ab nemo.'
    }
  }
}
</script>

<style scoped>

</style>
