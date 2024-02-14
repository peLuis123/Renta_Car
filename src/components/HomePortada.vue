<template>
  <v-container
    class="pa-0 ma-0 portada d-flex justify-center  align-center"
    style="height:auto; min-height: 500px"
    fluid
  >
    <div
      style="width: 1550px;"
      class="ma-5"
    >
      <v-row
        style="margin-top:90px;"
      >
        <v-col
          cols="12"
          md="8"
          sm="12"
        >
          <h1
            class="text-white"
            style="font-size: 60px;"
          >
            Rental Cars From Just
          </h1>
          <span
            class="text-orange"
            style="font-size: 60px;"
          >
            $25/Day
          </span>
        </v-col>
        <v-col
          cols="12"
          md="4"
          sm="12"
        >
          <ReservationPortada />
        </v-col>
      </v-row>
      <v-row>
        <v-col
          cols="12"
          md="4"
          sm="12"
        >
          <v-form>
            <v-row dense>
              <v-col

                cols="12"
                md="12"
              >
                <v-combobox

                  variant="solo-filled"
                  label="Car Type"
                  :items="['Car Type','Sedan','SUV','Van']"
                />
              </v-col>
              <v-col
                cols="12"
                md="12"
              >
                <v-text-field
                  label="Pick Up Location"
                  variant="solo-filled"
                />
              </v-col>
              <v-col
                cols="12"
                md="6"
              >
                <v-text-field
                  label="Pick Up Date"
                  variant="solo-filled"
                />
              </v-col>
              <v-col
                cols="12"
                md="6"
              >
                <v-text-field
                  label="Pick Up Time"
                  variant="solo-filled"
                />
              </v-col>
              <v-col
                cols="12"
                md="6"
              >
                <v-text-field
                  label="Drop off Date"
                  variant="solo-filled"
                />
              </v-col>
              <v-col
                cols="12"
                md="6"
              >
                <v-text-field
                  label="Drop off Time"
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
        <v-col
          cols="12"
          md="8"
          sm="12"
        >
          <div>
            <v-img

              src="https://www.elegantthemes.com/layouts/wp-content/uploads/2018/07/Car-Rental-Image-25.png"
            />
          </div>
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<script setup>
import ReservationPortada from '@/components/ReservationPortada.vue';
</script>
<style scoped>
.portada {
  background-image: linear-gradient(118deg, #063661 0%, rgba(43, 78, 136, 0.67) 100%), url(https://www.elegantthemes.com/layouts/wp-content/uploads/2018/06/car-dealer-35.jpg) !important;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center center;
}
</style>
