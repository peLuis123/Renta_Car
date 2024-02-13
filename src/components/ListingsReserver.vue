<template>
  <v-container
    class="d-flex justify-center flex-column"
    style="height: auto; max-width: 1250px; min-height: 300px;"
    fluid
  >
    <div>
      <h1
        class="ma-4 d-flex justify-start"
        style="font-size:50px;"
      >
        Resevering a Car is Easy!
      </h1>
      <div class="d-flex">
        <div
          v-for="(type) in types"
          :key="type.id"
          class="ma-5 d-flex justify-center"
        >
          <v-icon color="blue">
            mdi-circle-slice-8
          </v-icon>
          <h4>{{ type.name }}</h4>
        </div>
      </div>
      <v-divider />
    </div>
    <div class="d-flex flex-wrap justify-center ma-4">
      <div
        v-for="(item) in items"
        :key="item.id"
      >
        <CarDetails :item="item" />
      </div>
    </div>
  </v-container>
</template>
<script setup>
import { ref } from 'vue'
import CarDetails from './CarDetails.vue'
const types = ref([
    { id: 1, name: "Book Online, by Phone, or In Person", status: "true" },
    { id: 2, name: "Pick Up Vehicle or Request Pickup", status: "true" },
    { id: 3, name: "Enjoy Unlimited Driving Miles", status: "false" },
    { id: 4, name: "Drop Off at Valid Location & Pay", status: "true" }
])
const items = ref([
    {
        index: 1,
        image:"https://www.elegantthemes.com/layouts/wp-content/uploads/2018/07/Car-Rental-Image-26.jpg",
        title: "Monarch Sport",
        subtitle: "Starting $44/day",
        items: { type: "Sedan", blurb: "4 doords, 5 Seats", Transmission: "automatic" },
        show: "false",
        details: "Your content goes here. Edit or remove this text inline or in the module Content settings. You can also style every aspect of this content in the module Design settings and even apply custom CSS to this text in the module Advanced settings."
    },
    {
        index: 2,
        image:"https://www.elegantthemes.com/layouts/wp-content/uploads/2018/07/Car-Rental-Image-27.jpg",
        title: "Monarch Sport",
        subtitle: "Starting $44/day",
        items: { type: "SUV", blurb: "4 Doors, 7 Seats", Transmission: "Automatic" },
        show: "false",
        details: "Your content goes here. Edit or remove this text inline or in the module Content settings. You can also style every aspect of this content in the module Design settings and even apply custom CSS to this text in the module Advanced settings."
    },
    {
        index: 3,
        image:"https://www.elegantthemes.com/layouts/wp-content/uploads/2018/07/Car-Rental-Image-30.jpg",
        title: "Extra Explorer BB",
        subtitle: "Starting $44/day",
        items: { type: "SUV", blurb: "4 Doors, 4 Seats", Transmission: "Automatic" },
        show: "false",
        details: "Your content goes here. Edit or remove this text inline or in the module Content settings. You can also style every aspect of this content in the module Design settings and even apply custom CSS to this text in the module Advanced settings."
    },
    {
        index: 4,
        image:"https://www.elegantthemes.com/layouts/wp-content/uploads/2018/07/Car-Rental-Image-28.jpg",
        title: "Nexus Passenger",
        subtitle: "Starting $44/day",
        items: { type: "SUV", blurb: "4 Doors, 8 Seats", Transmission: "Automatic" },
        show: "false",
        details: "Your content goes here. Edit or remove this text inline or in the module Content settings. You can also style every aspect of this content in the module Design settings and even apply custom CSS to this text in the module Advanced settings."
    },
])
</script>
<style scoped>

</style>