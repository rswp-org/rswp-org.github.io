<template>
    <v-container class="size">
      <v-row cols="2">

        <v-col cols="12" md="6" class="pa-6">
          <v-row class="py-1">
            <h1>rainwater app</h1>
          </v-row>
          <v-row class="py-2">
            <p>Discover Rainwater—our free, web-based tool that makes designing and evaluating rainwater harvesting
              systems simple and effective. Using up to 40 years of historic rainfall data from trusted sources,
              Rainwater lets you:</p>
          </v-row>
          <v-row>
            <ul style="padding-left: 20px;">
              <li>
                <strong>Assess Local Rainfall:</strong> Quickly see how much rain falls in your area to establish a reliable base-case assumption.
              </li>
              <li>
                <strong>Tailor to Your Needs:</strong> Define the number of users and their water requirements to calculate the optimal capture surface area and storage volume.
              </li>
              <li>
                <strong>Forecast Performance:</strong> Instantly compare water supply against demand, whether you’re planning a new system or assessing an existing one.
              </li>
            </ul>
          </v-row>
          <v-row class="py-2">
            <p>By transforming complex data into actionable insights, Rainwater empowers communities and 
              organizations to build efficient, cost-effective water solutions. Join us in harnessing 
              nature’s bounty with smart, data-driven design.</p>
          </v-row>

          <v-row class="py-2">
            <v-btn class="text-none" color="#00aeef" rounded elevation="4" href="https://rswp.beehiiv.com/p/introducing-rainwater-a-free-to-use-app-for-rainwater-harvesting">learn more</v-btn>
          </v-row>
        </v-col>

        <v-col cols="12" md="6" class="pa-6">
          <v-row class="justify-end py-1">
            <v-img src="..\assets\rainwater_screenshot.PNG" class="rounded-lg"></v-img>
          </v-row>
        </v-col>

      </v-row>
    </v-container>
  </template>
  
  <script setup>
    //
  </script>
  
  <style>
  
  .size {
    max-width: 80%;
    justify-content: center;
  }
  
  </style>