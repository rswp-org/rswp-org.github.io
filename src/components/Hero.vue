<template>
  <v-container class="hero">
    <v-row class="ma-0" style="height: 100%;" cols="3" align="top" >
      <v-col style="height: 100%" >
        <v-img class="ma-5" src="../assets/RSWP_Logo_Horizontal_Inverse.svg"></v-img>
      </v-col>
      <v-col style="height: 100%">
        <v-row class="ma-5 justify-center">
          <v-btn class="text-none" color="#00aeef" style="align: center; min-width:33%" rounded><a href="#give">give</a></v-btn>
        </v-row>
      </v-col>
      <v-col class="ma-5" style="height: 100%">
        <v-row class="justify-end pa-4">
        <li style="text-align: right">
          <a href="https://github.com/rswp-org" target="_blank">
            <img style="max-width: 10%" src="../assets/github.svg" class="icon mx-1" />
          </a>
          <a href="https://instagram.com" target="_blank">
            <img style="max-width: 10%" src="../assets/instagram.svg" class="icon mx-1" />
          </a>
          <a href="https://www.linkedin.com/company/rural-schools-water-project" target="_blank">
            <img style="max-width: 10%" src="../assets/linkedin.svg" class="icon mx-1" />
          </a>
          <a href="https://youtube.com" target="_blank">
            <img style="max-width: 10%" src="../assets/youtube.svg" class="icon mx-1" />
          </a>
          </li>
        </v-row>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
        <v-row class="pa-8" cols="3" align="center">
          <p style="color: white; text-align: left"> We are a small charity using data and technology to build solutions for schools and communities facing water crises.<br><br>We’ve built 6 school water systems in Uganda since 2017—and we’re just getting started.</p>
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>

.hero {
  align: center;
  background: url("../assets/rswp_hero _bw_flip.JPG");
  background-size: cover;
  height: 100vh;
  max-width: 100vw;
}

.icons{
  max-width: 50%;
}

</style>