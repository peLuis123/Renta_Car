<template>
  <v-container
    class="contact-form "
    fluid
  >
    <div class="d-flex flex-column justify-center align-center">
      <div>
        <h1
          class="ma-5"
          style="font-size: 60px;"
        >
          Contact Us
        </h1>
      </div>
      <div
        style="max-width:1250px;"
        class="pa-4 ma-0 d-flex flex-row"
      >
        <div class="mr-10">
          <v-row>
            <v-col
              cols="12"
              sm="6"
            >
              <v-text-field
                label="Name"
                outlined
              />
            </v-col>
            <v-col
              cols="12"
              sm="6"
            >
              <v-text-field
                label="Email Address"
                outlined
              />
            </v-col>
            <v-col cols="12">
              <v-textarea
                label="Message"
                outlined
              />
            </v-col>
            <v-col cols="12">
              <v-btn
                color="orange"
                dark
              >
                Submit
              </v-btn>
            </v-col>
          </v-row>
        </div>
        <div class="d-flex flex-column">
          <div
            v-for="(item) in items"
            :key="item.value"
            class="ma-7"
          >
            <v-icon class="mr-3">
              {{ item.icon }}
            </v-icon> {{ item.title }}
          </div>
        </div>
      </div>
    </div>
  </v-container>
</template>
<script setup>
import { ref } from 'vue'
const items = ref([
    {
        title: 'pedrorc2018@gmail.com',
        icon: 'mdi-email',
        value: 1,
    },
    {
        title: '+51 958 104 634',
        value: 2,
        icon: 'mdi-phone-message',
    },
    {
        title: 'calle random 123 francia',
        value: 3,
        icon: 'mdi-map-marker',
    },
],)
</script>
<style scoped>
.contact-form {
    background-color: #3050d1;
    color: white;
    padding: 20px;
}
</style>
