<template>
  <!-- en caso que quieras crear un sidebard y un app-bar se agrega aqui y ya se aplican a todas las rutas hijas -->
  <v-app>
    <AppBar />
    <ViewLayout />
    <FooterComponent />
  </v-app>
</template>

<script setup>
import ViewLayout from './ViewLayout.vue'
import AppBar from '@/components/AppBar.vue'
import FooterComponent from '@/components/FooterComponent.vue'
</script>
