<template>
  <footer style="background-color: black">
    <v-row>
      <v-col cols="12" md="6" class="pa-6">
        <v-row class="pa-4">
          <v-img src="../assets/RSWP_Logo_Horizontal_Inverse.svg" max-width="250" height="auto" />
        </v-row>
        <v-row class="pa-4">
          <p style="color: white;">Registered Charity in England and Wales No. 1170858</p>
        </v-row>
      </v-col>
      <v-col cols="12" md="6" class="pa-6">
        <v-row class="justify-end pa-4">
          <p style="color: white;">hello@rswp.org</p>
        </v-row>
        <v-row class="justify-end pa-4">
          <!-- Wrap v-img in <a> tags to make them clickable -->
          <a href="https://github.com/rswp-org" target="_blank">
            <img src="../assets/github.svg" class="icon mx-1" />
          </a>
          <a href="https://instagram.com" target="_blank">
            <img src="../assets/instagram.svg" class="icon mx-1" />
          </a>
          <a href="https://www.linkedin.com/company/rural-schools-water-project" target="_blank">
            <img src="../assets/linkedin.svg" class="icon mx-1" />
          </a>
          <a href="https://youtube.com" target="_blank">
            <img src="../assets/youtube.svg" class="icon mx-1" />
          </a>
        </v-row>
      </v-col>
    </v-row>
  </footer>
</template>

<style scoped>
.icon {
  max-width: 30px;
  height: auto;
}

a {
  display: inline-block; /* Ensures the anchor has size */
  color: white; /* Inherits color (usually white) */
  text-decoration: none; /* Removes underline */
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
