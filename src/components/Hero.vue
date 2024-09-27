<template>
  <v-img class="hcard" src="../assets/rswp_hero _bw_flip.JPG">

    <v-row class="ma-0" style="height: 100%;" cols="3" align="top" >
      
      <v-col style="height: 100%; justify-content: space-evenly" > <!-- logo top corner -->
        <v-img class="ma-5" src="../assets/RSWP_Logo_Horizontal_Inverse.svg"></v-img>
      </v-col>

      <v-col style="height: 100%"> <!-- Button at top -->
        <v-row class="ma-5" style="justify-content: center">
          <v-btn color="#00aeef" style="align: center; min-width:33%" rounded>Give</v-btn>
        </v-row>
      </v-col>
    
      <v-col class="ma-5" style="height: 100%"> <!-- text -->
        <v-row class="justify-end">
          <v-img style="max-width: 15%" src="../assets/github.svg" class="icon mx-1" />
          <v-img style="max-width: 15%" src="../assets/instagram.svg" class="icon mx-1" />
          <v-img style="max-width: 15%" src="../assets/linkedin.svg" class="icon mx-1" />
          <v-img style="max-width: 15%" src="../assets/youtube.svg" class="icon mx-1" />
        </v-row>
      </v-col>
    </v-row>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
    <v-row style="align-items: end">
      <h2> Placeholder </h2>
    </v-row>
  </v-img>

</template>

<style scoped>

.hcard {
align-items: start;
top: 0;
left: 0;
max-width: 100%;
max-height: 100%;
}

.hcard img {
max-height: 50%;
max-width: 100%;
}

.icons{
  max-width: 50%;
}
</style>