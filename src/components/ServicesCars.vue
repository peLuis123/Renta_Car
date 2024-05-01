<template>
  <div
    v-for="(item,index) in items"
    :key="index"
    style="min-width: 250px; width: 350px;"
  >
    <div class=" d-flex pt-5 pb-5 letra">
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
</template>
<script setup>
import {ref} from 'vue'
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