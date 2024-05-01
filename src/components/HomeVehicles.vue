<template>
  <v-container
    style="height: auto; max-width: 1250px; min-height: 300px "
    class="d-flex justify-center align-center flex-column letra"
  >
    <div class="d-flex flex-wrap justify-center ma-4">
      <div
        v-for="(item) in items"
        :key="item.id"
      >
        <CarDetails
          :item="item"
        />
      </div>
    </div>
    <v-btn
      variant="outlined"
      color="blue"
    >
      BROWSE ALL VEHICLES
    </v-btn>
  </v-container>
</template>
<script setup>
import {ref} from 'vue'
import CarDetails from "./CarDetails"
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
])
</script>