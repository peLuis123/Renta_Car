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
        <h1 class="pb-2">
          Get Into Gear
        </h1>
        <div>
          Pellentesque in ipsum id orci porta dapibus. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices
          posuere cubilia Curae; Donec velit neque, auctor sit amet aliquam vel, ullamcorper sit amet ligula.
        </div>
      </div>
      <div class="d-flex flex-wrap justify-space-between">
        <div
          v-for="(item,index) in items"
          :key="index"
          style="min-width: 250px; width: 350px;"
        >
          <div class=" d-flex pt-5 pb-5">
            <div>
              <v-icon
                color="blue"
                size="38"
              >
                {{ item.icon }}
              </v-icon>
            </div>
            <div class="text-center">
              <span style="font-size: 18px; font-weight: bold;">{{ item.title }}</span>
              <p>{{ item.paragraf }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div

      style="width: auto; min-width: 350px  ;"
    >
      <h1 class="mb-5">
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
// import ReservationPortada from './ReservationPortada.vue';
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
const items = ref([
    {
        icon: 'mdi-tag-outline',
        title: 'The Lowest Rates',
        paragraf: 'Vestibulum id ligula porta felis euismod semper. Donec ullamcorper nulla non metus auctor fringilla.'
    },
    {
        icon: 'mdi-key-variant',
        title: 'Unlimited Gas & Miles',
        paragraf: 'Nulla quis lorem ut libero malesuada feugiat. Arcu erat, accumsan id imperdiet et, porttitor'
    },
    {
        icon: 'mdi-clock-time-five',
        title: '24/7 Pickup & Return Access',
        paragraf: 'Nulla quis lorem ut libero malesuada feugiat. Arcu erat, accumsan id imperdiet et, porttitor'
    },
    {
        icon: 'mdi-map-marker-outline',
        title: 'Multiple Drop-Off Locations',
        paragraf: 'Nulla quis lorem ut libero malesuada feugiat. Arcu erat, accumsan id imperdiet et, porttitor'
    },
])
</script>
