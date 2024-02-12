<template>
  <!-- en caso que quieras crear un sidebard y un app-bar se agrega aqui y ya se aplican a todas las rutas hijas -->
  <v-app>
    <default-view />
  </v-app>
</template>

<script setup>
import { ref } from 'vue';
  import DefaultView from './View.vue'
  // const hora =  Date.time
  const count = ref(0)
  console.log(count)
  // console.log(hora)
  // function hora(){

  // }
</script>
