<template>
  <v-container
    class="pa-0 ma-0 portada"
    fluid
  >
    <div
      class="pa-4 ma-0 d-flex flex-column justify-center align-center"
      style="height: auto; max-width: 100%; min-height: 500px;"
    >
      <h1>Satisfaction Guaranteed</h1>
      <div
        class="d-flex flex-wrap justify-center align-center"
        style="max-width: 1250px;"
      >
        <div
          v-for="(item) in items"
          :key="item.id"
          class="text-white ma-10"
          style="font-size: 18px;"
        >
          <CheckList :item="item" />
        </div>
      </div>
    </div>
  </v-container>
</template>

<script setup>
import CheckList from './CheckList.vue';
import { ref } from 'vue'
const items = ref([
    {
        id: 1,
        text: "Curabitur arcu erat, accumsan id imperdiet et"
    },
    {
        id: 2,
        text: "Curabitur arcu erat, accumsan id imperdiet et"
    },
    {
        id: 3,
        text: "Curabitur arcu erat, accumsan id imperdiet et"
    },
    {
        id: 4,
        text: "Curabitur arcu erat, accumsan id imperdiet et"
    },
    {
        id: 5,
        text: "Curabitur arcu erat, accumsan id imperdiet et"
    },
    {
        id: 6,
        text: "Curabitur arcu erat, accumsan id imperdiet et"
    },
])
</script>
<style scoped>
.portada {
    background-image: linear-gradient(118deg, #063661 0%, rgba(43, 78, 136, 0.67) 100%), url(https://www.elegantthemes.com/layouts/wp-content/uploads/2018/06/car-dealer-25.jpg) !important;
    background-size: cover;
    background-repeat: no-repeat;
    height: auto;
    background-position: center center;
}
</style>
