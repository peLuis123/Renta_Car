<template>
  <v-container
    class=" portada d-flex justify-center text-white letra"
    style="height:auto; min-height: 700px"
    fluid
  >
    <div
      class="d-flex  align-center justify-center flex-column"
      style="width: 1080px;"
    >
      <div
        class="text-center ma-5"
        style="font-size:35px;"
      >
        <h1>Our Lot is Open 24/7</h1>
        <h2 class="text-orange">
          +51 958 104 634
        </h2>
      </div>
      <div
        class="d-flex flex-row justify-space-between flex-wrap ma-5"
        style="min-width: 350px; font-size: 20px;"
      >
        <ContactInfo />
      </div>
      <div class="ma-5">
        <v-btn
          height="55px"
          color="#faa152"
          class="btn-reserve text-white"
        >
          RESERVE A CAR ONLINE
        </v-btn>
      </div>
    </div>
  </v-container>
</template>

<script setup>
import ContactInfo from './ContactInfo.vue';
</script>
<style scoped>

.portada {
    background-image: linear-gradient(118deg, #063661 0%, rgba(43, 78, 136, 0.67) 100%), url(https://www.elegantthemes.com/layouts/wp-content/uploads/2018/07/Car-Rental-Image-29.jpg) !important;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
}
</style>
