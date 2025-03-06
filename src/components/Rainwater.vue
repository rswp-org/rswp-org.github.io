<template>
  <v-container fluid class="component-background">
    <v-container class="rainwater-card my-16 px-8 py-10" style="border-radius: 20px; overflow: hidden; min-height: 600px;">
      <v-row cols="2" class="px-4">
        <v-col cols="12" md="6" class="pa-6">
          <v-row class="fill-height" align="center" justify="center">
            <v-sheet
              width="400"
              height="400"
              color="rgba(0, 0, 0, 0.8)"
              style="border-radius: 20px; overflow: hidden;"
            >
              <v-img
                src="../assets/rainwater_plot.png"
                width="400"
                height="400"
                class="rounded-lg"
                contain
              ></v-img>
            </v-sheet>
          </v-row>
        </v-col>
        <v-col cols="12" md="6" class="pa-6">
          <v-row class="py-1 my-5">
            <h1 style="color: white">Rainwater supply forecasting</h1>
          </v-row>
          <v-row class="py-2 mt-8">
            <p style="color: white; font-size: 17px; text-align: left">Discover Rainwater—our free, web-based tool for designing and evaluating rainwater harvesting
              systems.</p>
          </v-row>
          <v-row class="mt-8">
            <v-col cols="12" class="pa-0">
              <ul class="text-white" style="list-style: none !important; padding-left: 0;">
                <li class="flex items-center gap-2 mb-2">
                  <v-icon color="green" class="mr-2">mdi-check</v-icon>
                  <span>Choose rainfall scenarios aligned to your risk preference</span>
                </li>
                <li class="flex items-center gap-2 mb-2">
                  <v-icon color="green" class="mr-2">mdi-check</v-icon>
                  <span>Instantly forecast supply versus demand</span>
                </li>
                <li class="flex items-center gap-2 mb-2">
                  <v-icon color="green" class="mr-2">mdi-check</v-icon>
                  <span>Determine optimal capture area and storage requirements</span>
                </li>
              </ul>
            </v-col>
          </v-row>
          <!-- Action Links -->
          <v-row>
            <v-col cols="12" class="pa-0">
              <div class="my-8 flex">
                <a 
                  href="https://rswp.beehiiv.com/p/introducing-rainwater-a-free-to-use-app-for-rainwater-harvesting" 
                  target="_blank" 
                  class="find-out-more text-sm font-semibold leading-6"
                >
                  Find out more <span aria-hidden="true">→</span>
                </a>
                <span class="mx-4"></span>
                <a 
                  href="https://rswp.beehiiv.com/p/introducing-rainwater-a-free-to-use-app-for-rainwater-harvesting" 
                  target="_blank" 
                  class="watch-the-demo text-sm font-semibold leading-6"
                >
                  Watch the demo <span aria-hidden="true">→</span>
                </a>
              </div>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
  </template>
  
  <script setup>

  </script>

<style scoped>

  .component-background {
    background: rgba(44, 44, 44, 1);
  }

  .rainwater-card {
    max-width: 80%;
    justify-content: center;
    background-color: rgba(0, 0, 0, 0.5);
    align-content: center;
  }

  .find-out-more {
  color: #00aeef;
  }

  .find-out-more:hover {
    color: rgb(152, 229, 255);
  }

  .watch-the-demo {
  color: #ffffff;
  }

  .watch-the-demo:hover {
    color: rgb(163, 163, 163);
  }

</style>