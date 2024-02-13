<template>
  <div class="d-flex align-center flex-column ">
    <v-card
      class=" ma-4 "
      width="342px"
      min-width="250px"
    >
      <v-img
        :src="item.image"
        height="200px"
        cover
      />
      <v-card-title
        style="font-weight:bold"
      >
        {{ item.title }}
      </v-card-title>
      <v-card-subtitle
        class="pb-4 text-orange"
        style="font-weight:bold"
      >
        {{ item.subtitle }}
      </v-card-subtitle>
      <v-divider />
      <v-card-text>
        <div class="text-subtitle-1">
          <v-icon
            class="mr-3"
            color="blue"
          >
            mdi-key-variant
          </v-icon> Vehicle Type: {{ item.items.type }}
        </div>
        <div class="my-4 text-subtitle-1">
          <v-icon
            class="mr-3"
            color="blue"
          >
            mdi-account-multiple
          </v-icon> {{ item.items.blurb }}
        </div>
        <div class="my-4 text-subtitle-1">
          <v-icon
            class="mr-3"
            color="blue"
          >
            mdi-cog
          </v-icon> Transmission: {{ item.items.Transmission }}
        </div>
      </v-card-text>
      <v-divider />
      <v-card-actions>
        <h4>More Details</h4>
        <v-spacer />
        <v-btn
          :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'"
          @click="show = !show"
        />
      </v-card-actions>

      <v-expand-transition class="pb-5">
        <div v-show="show">
          <v-card-text>
            {{ item.details }}
          </v-card-text>
        </div>
      </v-expand-transition>
    </v-card>
    <v-btn
      height="55px"
      color="#faa152"
      class="btn-reserve text-white"
    >
      RESERVE NOW
    </v-btn>
  </div>
</template>
<script setup>
import { ref,defineProps } from 'vue'
defineProps({
  item:{type: Object, default: () =>{}}
})
const show = ref("false")

</script>
<style scoped>
.btn-reserve{
  top:-33px;
}

</style>