<template>
  <v-container
    style="height: auto;  min-height: 300px"
    class="d-flex justify-center align-center flex-column letra ma-15 "
  >
    <div
      class="d-flex flex-column justify-center align-center flex-wrap"
      style="height: auto;  width:1250px; min-width: 350px; background-color: blue;  "
    >
      <div>
        <h1 style="font-size:60px">
          Renting A Car Has Never Been Easier
        </h1>
      </div>
      <div
        class="d-flex flex-wrap flex-row justify-center"
      >
        <InfoComponent :color="color" />
      </div>
    </div>
  </v-container>
</template>

<script setup>
import InfoComponent from './InfoComponent.vue';
const color='orange'
</script>