<template>
    
    <v-img class="hcard" src="../assets/rswp_hero _bw_flip.JPG">
      <v-row class="ma-0" style="height: 100%;" cols="3" align="start" >

      <v-col style="height: 100%;" > <!-- logo top corner -->
        <v-img class="ma-5" src="../assets/RSWP_Logo_Horizontal_Inverse.svg"></v-img>
      </v-col>

      <v-col style="height: 100%; align-items: center;"> <!-- Button at top -->
        <v-btn color="#e033" style="justify-content: center;" rounded>Give</v-btn>
      </v-col>
      
      <v-col class="ma-0" style="height: 100%;"> <!-- text -->

          <v-row style="justify-content: end;">
                <img style="max-width: 15%; align-items: center; margin-right: 5px; margin-top: 5px;" src="../assets/github.svg"/>
                <img style="max-width: 15%; align-items: center; margin-right: 5px; margin-top: 5px"  src="../assets/instagram.svg"/>
                <img style="max-width: 15%; align-items: center; margin-right: 5px; margin-top: 5px"  src="../assets/youtube.svg"/>
          </v-row>

          <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
          <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

          <v-row>
            <h2> Placeholder </h2>
          </v-row>

      </v-col>
     </v-row >
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