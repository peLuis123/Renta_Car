<template>
  <v-app-bar
    :elevation="2"
    class="letra"
  >
    <v-app-bar-title>Renta Car</v-app-bar-title>
    <div
      v-for="(item) in items"
      :key="item.id"
    >
      <v-btn
        variant="plain"
        :to="item.to"
      >
        {{ item.text }}
      </v-btn>
    </div>

    <v-icon class="ma-5">
      mdi-cart
    </v-icon>
  </v-app-bar>
</template>
<script setup>
import { ref } from 'vue'
const items = ref([
    { id: 1, text: 'home', to: "/home" },
    { id: 2, text: 'listings', to: "/listings" },
    { id: 3, text: 'contact', to: "/contact" },
    { id: 4, text: 'landing', to: "/landing" },
    { id: 5, text: 'services', to: "/listings" },
    { id: 6, text: 'about', to: "/listings" },
    { id: 7, text: 'listing', to: "/listings" }
]);
</script>
