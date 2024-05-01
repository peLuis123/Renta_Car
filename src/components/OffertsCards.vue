<template>
  <v-card
    class="letra ma-2 pa-2 d-flex align-center"
    style="width: auto; min-width: 120px; "
  >
    <div
      class="pa-5"
    >
      <v-icon
        size="35"
        color="#faa152"
      >
        mdi-tag
      </v-icon>
    </div>
    <div
      class="text-center"
      style="width: 80%;"
    >
      <h1>{{ offert.discount }}</h1>
      <div>{{ offert.infoExtra }}</div>
    </div>
  </v-card>
</template>
<script setup>
defineProps({
    offert:{type: Object, default: () =>{}}
  })
</script>
