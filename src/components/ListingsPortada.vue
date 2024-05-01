<template>
  <v-container
    class="pa-0 ma-0 portada d-flex justify-center  align-center letra"
    style="height:auto; min-height: 500px ;"
    fluid
  >
    <div
      class="pa-4 ma-0 d-flex flex-wrap"
      style="height: 100%;"
    >
      <div>
        <div>
          <h1
            class="text-white mr-15"
            style="font-size: 60px;"
          >
            Available Cars For Rent
          </h1>
          <span
            class="text-orange"
            style="font-size: 60px;  font-weight: bold; "
          >As Low as $25/day</span>
        </div>
        <v-btn color="orange-darken-3">
          SPEACK WITH AGENT
        </v-btn>
      </div>
      <ReservationPortada />
    </div>
  </v-container>
</template>

<script setup>
import ReservationPortada from '@/components/ReservationPortada.vue';
</script>
<style scoped>
.portada {
  background-image: linear-gradient(118deg, #063661 0%, rgba(43, 78, 136, 0.67) 100%), url(https://www.elegantthemes.com/layouts/wp-content/uploads/2018/07/Car-Rental-Image-29.jpg) !important;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
}

</style>
