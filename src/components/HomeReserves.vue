<template>
  <v-container
    style="min-height: 300px;"
    class="d-flex  justify-center align-center letra"
  >
    <div class="d-flex flex-row justify-center flex-wrap">
      <InfoComponent :color="color" />
    </div>
  </v-container>
</template>
<script setup>
import InfoComponent from './InfoComponent.vue';
const color='blue'
</script>
