<template>
  <v-container class="hero">
    <v-row class="ma-0" style="height: 50%;" cols="3"  >
      <v-col style="height: 100%; max-width: 50%;" >
        <img class="img" src="../assets/RSWP_Logo_Horizontal_Inverse.svg"></img>
      </v-col>
      <v-col style="height: 100%; max-width: 25%;">
        <v-row style="" class="ma-5 justify-center">
          <v-btn class="text-none" color="#00aeef" style="align: center; min-width:33%" rounded><a href="#give">give</a></v-btn>
        </v-row>
      </v-col>
      <v-col class="ma-5" style="height: 100%; max-width: 25%;">
        <v-row style="align-items: right;" align-right class="justify-end pa-4">
        <li style="text-align: right;  list-style-type: none; vertical-align: top;">
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
            <img style="max-width: 10%;" src="../assets/youtube.svg" class="icon mx-1" />
          </a>
        </li>
        </v-row>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
       
      </v-col>
     
    </v-row>
        <v-row style="float: right; max-width: 750px" class="pa-8" cols="3" align="end">
          <p style="align-items: end; color: white; text-align: right"> We are a small charity using data and technology to build solutions for schools and communities facing water crises.<br><br>We’ve built 6 school water systems in Uganda since 2017—and we’re just getting started.</p>
        </v-row>
  </v-container>
</template>

<style scoped>

.hero {
  align: center;
  background: url("../assets/rswp_hero _bw_flip.JPG");
  background-size: cover;
  height: 100vh;
  max-width: 100%;
  object-fit: cover;
}


.img{
   position: relative;
}

</style>