<template>
  <v-container
    fluid
    style="max-width: 1280px; width: auto;"
    class="d-flex flex-row flex-wrap justify-space-between"
  >
    <div
      style="max-width: 810px;"
      class="d-flex flex-column"
    >
      <div class="pt-5 pb-5">
        <h1 class="pb-2 letra">
          Get Into Gear
        </h1>
        <div class="letra">
          Pellentesque in ipsum id orci porta dapibus. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices
          posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet ligula.
        </div>
      </div>
      <div class="d-flex flex-wrap justify-space-between">
        <ServicesCars />
      </div>
    </div>
    <div

      style="width: auto; min-width: 350px  ;"
    >
      <h1 class="mb-5 letra">
        Offerts
      </h1>
      <div>
        <OffertsCards
          v-for="(offert, index) in offerts"
          :key="index"
          :offert="offert"
        />
      </div>
    </div>
  </v-container>
</template>

<script setup>
import {ref} from 'vue'
import OffertsCards from './OffertsCards.vue';
import ServicesCars from './ServicesCars.vue';
const offerts = ref([
    {
        discount:"15% Off",
        infoExtra:"First Time Reservations"
    },
    {
        discount:"8% Off",
        infoExtra:"4+ Day Reservations"
    },
    {
        discount:"10% Off",
        infoExtra:"Passenger Van Rentals"
    }
])

</script>
