<template>
    <v-container rounded style="max-width: 1400px;" justify="center" fluid>
      <v-card rounded justify="center" color="primary" elevation="4"> 
       
          <v-row justify="center" class="ma-1">
            <h1 style="justify-content: center; color: white;" justify="center" align="center"> the team</h1>
          </v-row>

          <v-row class="ma-4" justify="center">
            <p style="justify-content: center; color: white;" justify="center" align="center"> we are small team based around the world. focused on delivering the best water solutions in afica.</p>

            <v-hover v-slot="{ isHovering, props }">
              <v-card v-bind="props" class="teamCard ma-2" rounded outlined elevation="4">   
                <v-fade-transition leave-absolute="true">
                  <div class="card_reveal ma-6" v-if="isHovering" >
                    <h3 style="font-size: 150%; color: #2c2c2c;">  I’m matt, I joined the board of trustees in 2022 and took over the financial side of rswp. </h3>                
                  </div>    
                  <div class="ma-6">
                    <v-img class="teamIcons" src="../assets/will.png"> </v-img>
                      <h2> matt coote </h2>
                        <h3 style="font-size: 150%;" class="water">finance lead</h3>    
                    </div> 
                </v-fade-transition>
              </v-card>
            </v-hover>

            <v-hover v-slot="{ isHovering, props }">
              <v-card v-bind="props" class="teamCard ma-2" rounded outlined elevation="4">   
                <v-fade-transition leave-absolute="true">
                  <div class="card_reveal ma-6" v-if="isHovering" >
                    <h3 style="font-size: 150%; color: #2c2c2c;">  I’m matt, I joined the board of trustees in 2022 and took over the financial side of rswp. </h3>                
                  </div>    
                  <div class="ma-6">
                    <v-img class="teamIcons" src="../assets/sharon.png"> </v-img>
                      <h2> matt coote </h2>
                        <h3 style="font-size: 150%;" class="water">finance lead</h3>    
                    </div> 
                </v-fade-transition>
              </v-card>
            </v-hover>

            <v-hover v-slot="{ isHovering, props }">
              <v-card v-bind="props" class="teamCard ma-2" rounded outlined elevation="4">   
                <v-fade-transition leave-absolute="true">
                  <div class="card_reveal ma-6" v-if="isHovering" >
                    <h3 style="font-size: 150%; color: #2c2c2c;">  I’m matt, I joined the board of trustees in 2022 and took over the financial side of rswp. </h3>                
                  </div>    
                  <div class="ma-6">
                    <v-img class="teamIcons" src="../assets/isobel.png"> </v-img>
                      <h2> matt coote </h2>
                        <h3 style="font-size: 150%;" class="water">finance lead</h3>    
                    </div> 
                </v-fade-transition>
              </v-card>
            </v-hover>

            <v-hover v-slot="{ isHovering, props }">
              <v-card v-bind="props" class="teamCard ma-2" rounded outlined elevation="4">   
                <v-fade-transition leave-absolute="true">
                  <div class="card_reveal ma-6" v-if="isHovering" >
                    <h3 style="font-size: 150%; color: #2c2c2c;">  I’m matt, I joined the board of trustees in 2022 and took over the financial side of rswp. </h3>                
                  </div>    
                  <div class="ma-6">
                    <v-img class="teamIcons" src="../assets/will.png"> </v-img>
                      <h2> matt coote </h2>
                        <h3 style="font-size: 150%;" class="water">finance lead</h3>    
                    </div> 
                </v-fade-transition>
              </v-card>
            </v-hover>

          </v-row>
      
  </v-card>

</v-container>
</template>

<script setup>

</script>

<style scoped>
.teamCard{
  text-align: center;
  height: 400px; 
  width: 300px;
  align-content: center;
  color:white;
  border-radius: 10%;
  position: relative;
}

.box{
 position: relative;
}

.card_reveal {
color:#00aeef;
text-align: center;
}

.teamIcons{
border-radius: 50%;
height: 250px;
width: 250px;
position: relative;
}

</style>
