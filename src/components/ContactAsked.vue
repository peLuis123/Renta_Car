<template>
  <v-container class="d-flex justify-center align-center">
    <div
      style="min-height: 300px; max-width: 1080px; min-width: 350px;"
      class="d-flex   flex-column flex-wrap"
    >
      <div class="text-center">
        <h1>Frequently Asked</h1>
      </div>
      <div class="d-flex flex-row flex-wrap justify-center">
        <v-card
          v-for="(item, index) in items"
          :key="index"
          class="pa-5 ma-5 d-flex"
          style="max-width: 500px; min-width: 150px; height: auto; "
        >
          <div>
            <v-icon
              color="blue"
              size="15"
              class="mr-3"
            >
              mdi-square
            </v-icon>
          </div>
          <div class="d-flex flex-wrap">
            <h2 style="font-size: 18px;">
              {{ item.ask }}
            </h2>
            <p style="font-size: 15px;">
              {{ item.answer }}
            </p>
          </div>
        </v-card>
      </div>
    </div>
  </v-container>
</template>
<script setup>
import { ref } from 'vue'
const items = ref([
  {
    ask: 'Quisque velit nisi pretium ut lacinia in?',
    answer: 'Vestibulum id ligula porta felis euismod semper. Donec ullamcorper nulla non metus auctor fringilla. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Nulla vitae elit libero, a pharetra augue. Etiam porta sem malesuada magna mollis euismod. Donec id elit non mi porta gravida at eget metus. Aenean lacinia bibendum nulla sed consectetur.'
  },
  {
    ask: 'Cras ultricies ligula sed magna dictum porta?',
    answer: 'Vestibulum id ligula porta felis euismod semper. Donec ullamcorper nulla non metus auctor fringilla. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Nulla vitae elit libero, a pharetr'
  },
  {
    ask: 'Pellentesque in ipsum id orci porta dapibus?',
    answer: 'Vestibulum id ligula porta felis euismod semper. Donec ullamcorper nulla non metus auctor fringilla. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Nulla vitae elit libero, a pharetra augue.'
  },

  {
    ask: 'Quisque velit nisi pretium ut lacinia in?',
    answer: 'Etiam porta sem malesuada magna mollis euismod. Donec id elit non mi porta gravida at eget metus. Aenean lacinia bibendum nulla sed consectetur.'
  },

  {
    ask: 'Mauris blandit aliquet elit eget tincidunt nibh pulvinar?',
    answer: 'Vestibulum id ligula porta felis euismod semper. Donec ullamcorper nulla non metus auctor fringilla. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Nulla vitae elit libero, a pharetr'
  },



  {
    ask: 'Vestibulum ac diam sit amet quam vehicula elementum?',
    answer: 'Vestibulum id ligula porta felis euismod semper. Donec ullamcorper nulla non metus auctor fringilla. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Nulla vitae elit libero, a pharetra augue. '
  },
  {
    ask: 'Quisque velit nisi pretium ut lacinia in?',
    answer: 'Etiam porta sem malesuada magna mollis euismod. Donec id elit non mi porta gravida at eget metus. Aenean lacinia bibendum nulla sed consectetur.'
  },
  {
    ask: 'Quisque velit nisi pretium ut lacinia in?',
    answer: 'Vestibulum id ligula porta felis euismod semper. Donec ullamcorper nulla non metus auctor fringilla. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Nulla vitae elit libero, a pharetra augue. Etiam porta sem malesuada magna mollis euismod. Donec id elit non mi porta gravida at eget metus. Aenean lacinia bibendum nulla sed consectetur.'
  },
])
</script>
