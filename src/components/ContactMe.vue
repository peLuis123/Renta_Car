<template>
  <v-container
    class="contact-form letra"
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
        class="pa-4 ma-0 d-flex flex-row flex-wrap"
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
                color="#faa152"
                dark
              >
                Submit
              </v-btn>
            </v-col>
          </v-row>
        </div>
        <div class="d-flex flex-column">
          <ContactInfo />
        </div>
      </div>
    </div>
  </v-container>
</template>
<script setup>
import ContactInfo from './ContactInfo.vue';
</script>
<style scoped>
.contact-form {
    background-color: #3050d1;
    color: white;
    padding: 20px;
}
</style>
