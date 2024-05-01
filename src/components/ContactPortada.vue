<template>
  <v-container
    class=" portada d-flex justify-center  align-center letra"
    style="height:auto; min-height: 500px"
    fluid
  >
    <div
      class="ma-4"
      style="width: 1080px; margin: 80px auto; "
    >
      <v-row>
        <v-col
          cols="12"
          md="8"
          sm="12"
        >
          <div class="text-white">
            <h1 style="font-size:60px;">
              Contact Us
            </h1>
            <p style="font-size:18px;">
              Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Vestibulum id ligula porta
              felis euismod semper. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh,
              ut fermentum massa justo sit am.
            </p>
          </div>
        </v-col>
        <v-col
          cols="12"
          md="4"
          sm="12"
        >
          <v-form>
            <v-row dense>
              <v-col
                cols="12"
                md="6"
              >
                <v-text-field
                  label="Name"
                  variant="solo-filled"
                />
              </v-col>
              <v-col
                cols="12"
                md="6"
              >
                <v-text-field
                  label="Email Address"
                  variant="solo-filled"
                />
              </v-col>
              <v-col
                cols="12"
                md="12"
              >
                <v-textarea
                  label="Message"
                  variant="solo-filled"
                />
              </v-col>
            </v-row>
            <v-row>
              <v-col
                cols="12"
                md="7"
              >
                <v-btn
                  height="45"
                  width="200"
                  color="orange-darken-3"
                >
                  Request Now
                </v-btn>
              </v-col>
            </v-row>
          </v-form>
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<script setup>

</script>
<style scoped>
.portada {
    background-image: linear-gradient(118deg, #063661 0%, rgba(43, 78, 136, 0.67) 100%), url(https://www.elegantthemes.com/layouts/wp-content/uploads/2018/07/Car-Rental-Image-21.jpg) !important;
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
}
</style>
