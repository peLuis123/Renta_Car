<template>
  <v-icon
    size="32px"
    color="orange"
    class="mr-2"
  >
    mdi-check-circle
  </v-icon> {{ item.text }}
</template>
<script setup>
import { defineProps } from 'vue';
defineProps({
  item:{type: Object, default: () =>{}}
})
</script>