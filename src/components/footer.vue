<template>
    <footer style="background-color: black">
      <v-row>
        <v-col>
          <v-row class="pa-4">
            <v-img src="../assets/RSWP_Logo_Horizontal_Inverse.svg" max-width="250" height="auto" />
          </v-row>
          <v-row class="pa-4">
            <h5 style="color: white;">Registered Charity in England and Wales No. 1170858</h5>
          </v-row>
        </v-col>
        <v-col>
          <v-row class="justify-end pa-4">
            <h5 style="color: white;">hello@rswp.org</h5>
          </v-row>
          <v-row class="justify-end pa-4">
            <!-- icons -->
            <v-img src="../assets/github.svg" class="icon mx-1" />
            <v-img src="../assets/instagram.svg" class="icon mx-1" />
            <v-img src="../assets/linkedin.svg" class="icon mx-1" />
            <v-img src="../assets/youtube.svg" class="icon mx-1" />
            </v-row>
        </v-col>
      </v-row>
    </footer>
  </template>
  
  <script setup>
    //
  </script>
  
  <style>
  .icon {
    max-width: 30px;
    height: auto;
  }

  footer {
  align-items: center;
  background-color: #00aeef;
  border-radius: 0.1rem 0.1rem 0rem 0rem;
  color: white;
  display: flex;
  flex-wrap: nowrap;
  justify-content: space-between;
  padding: 3.75rem;
}
  </style>