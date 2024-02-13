<template>
  <v-container
    style="min-height: 300px;"
    class="d-flex  justify-center align-center "
  >
    <div class="d-flex flex-row justify-center flex-wrap">
      <div
        v-for="(item) in items"
        :key="item.id"
        class="mr-15 ml-15 d-flex flex-column align-center"
      >
        <v-icon
          class="mb-4"
          size="80"
          color="blue"
        >
          {{ item.icon }}
        </v-icon>
        <h1 class="mb-0">
          {{ item.title }}
        </h1>
        <p class="mb-4">
          {{ item.subtitle }}
        </p>
        <v-btn
          color="blue"
          class="mb-4"
        >
          {{ item.action }}
        </v-btn>
      </div>
    </div>
  </v-container>
</template>
<script setup>
import { ref } from 'vue'
const items = ref([
    {
        id: '1',
        icon: 'mdi-tag',
        title: '15% Off',
        subtitle: 'first time Reservations',
        action: 'REDEEM'

    },
    {
        id: '2',
        icon: 'mdi-phone',
        title: 'Reserve by Phone',
        subtitle: 'Call Us 24/7',
        action: '+1 (233) 596-3496'

    },
    {
        id: '3',
        icon: 'mdi-television',
        title: 'Reserve Online',
        subtitle: 'In Just a Few Clicks',
        action: 'GET STARTED'

    }
])
</script>