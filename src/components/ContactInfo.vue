<template>
  <div
    v-for="(item) in items"
    :key="item.value"
    class="ma-7"
  >
    <v-icon class="mr-3">
      {{ item.icon }}
    </v-icon> <span class="letra">{{ item.title }}</span>
  </div>
</template>
<script setup>
import { ref } from 'vue'
const items = ref([
    {
        title: 'pedrorc2018@gmail.com',
        icon: 'mdi-email',
        value: 1,
    },
    {
        title: '+51 958 104 634',
        value: 2,
        icon: 'mdi-phone-message',
    },
    {
        title: 'calle random 123 francia',
        value: 3,
        icon: 'mdi-map-marker',
    },
],)
</script>