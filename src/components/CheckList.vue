<template>
  <v-icon
    size="32px"
    color="#faa152"
    class="mr-2"
  >
    mdi-check-circle
  </v-icon> <span class="letra">{{ item.text }}</span>
</template>
<script setup>
import { defineProps } from 'vue';
defineProps({
  item:{type: Object, default: () =>{}}
})
</script>