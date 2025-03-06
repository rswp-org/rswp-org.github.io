<template>
  <v-container class="hero">
    <v-row class="ma-2" style="height: 55%; justify-content: space-between;" cols="2"  >
      <v-col md="6" class="pa-6">
        <v-row class="pa-4">
        <v-img src="../assets/RSWP_Logo_Horizontal_Inverse.svg" max-width="300" height="auto" />
        </v-row>
      </v-col>
      <v-col md="6" class="pa-6">
        <v-row class="justify-end pa-4">
          <!-- Social Links -->
          <a href="https://github.com/rswp-org" target="_blank">
            <img
              style="width: 40px; height: 40px;" 
              src="../assets/github.svg" 
              class="icon mx-1" 
            />
          </a>
          <a href="https://www.instagram.com/rswp_org" target="_blank">
            <img
              style="width: 40px; height: 40px;" 
              src="../assets/instagram.svg" 
              class="icon mx-1" 
            />
          </a>
          <a href="https://www.linkedin.com/company/rural-schools-water-project" target="_blank">
            <img
              style="width: 40px; height: 40px;" 
              src="../assets/linkedin.svg" 
              class="icon mx-1" 
            />
          </a>
          <a href="https://www.youtube.com/@rswp-org" target="_blank">
            <img
              style="width: 40px; height: 40px;" 
              src="../assets/youtube.svg" 
              class="icon mx-1" 
            />
          </a>
        </v-row>
        <v-row class="justify-end pa-4">
          <v-btn class="text-none" color="#00aeef" style="min-height: 40px; width: 192px;" rounded><a href="#give">give</a></v-btn>
        </v-row>
      </v-col>
    </v-row>
    <v-row class="ma-0 pa-4" style="height: 45%;">
      <v-col class="d-flex flex-column justify-start" style="height: 100%; min-width: 25%;">
        <h2 style="color: white; text-align: center; font-family: ProximaNova-Bold">
          We use data and technology to support schools and communities facing 
          <span class="highlight">
          water crises
          </span>
        </h2>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>

.hero {
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), 
  url("../assets/rswp_hero _bw_flip.JPG") center fixed;
  background-size: cover;
  height: 100vh;
  max-width: 100%;
  object-fit: cover;
  padding: 1rem;
}

.img {
   position: relative;
}

</style>