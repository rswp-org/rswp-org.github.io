<template>
    <v-container rounded style="max-width: 1400px;" justify="center" fluid>

      <v-card rounded justify="center" color="primary" elevation="4"> 
       
          <v-row justify="center" class="ma-6">
            <h1 style="justify-content: center; color: white;" justify="center" align="center">the team</h1>
          </v-row>

          <v-row class="ma-4" justify="center">
            <v-container justify-center style="max-width: 1000px;">
              <h3 style="justify-content: center; color: white;" justify="center" align="center">rswp is run by an international team. We have a board of trustees who plan and manage our activities, and we work with local Ugandan partners to deliver projects. Find out more about each of our trustees below.</h3>
            </v-container>
          </v-row>

          <v-row  class="ma-4" justify="center">

            <v-hover v-slot="{ isHovering, props }">
              <v-card v-bind="props" class="teamCard ma-2" rounded outlined elevation="4">   
                <v-fade-transition hide-on-leave="true">
                  <div  class="card_reveal ma-6" v-if="isHovering" >
                    <v-img class="teamIconsSelected" src="../assets/will.png"> </v-img>
                    <div class="textTeam">
                      <h3 style="font-size: 100%; color: #2c2c2c;">Hey! I’m Will and I have the privilege of leading our amazing board of trustees. </h3>
                        <br>
                      <h3 style="font-size: 100%; color: #2c2c2c;">I’ve been part of RSWP since 2014 and I’m heavily involved in leading our projects and partnerships.</h3>
                        <br>
                      <h3 style="font-size: 100%; color: #2c2c2c;">I work at Save the Children International and study part-time at the Water Engineering and Development Centre (WEDC), Loughborough University. </h3> 
                    </div>   
                  </div> 
                  <div class="ma-12">
                    <v-img class="teamIcons" src="../assets/will.png"> </v-img>
                      <h2> will knapman </h2>
                        <h3 style="font-size: 150%;" class="water">co-found, chair and operations lead</h3>    
                    </div> 
                </v-fade-transition>
              </v-card>
            </v-hover>

            <v-hover v-slot="{ isHovering, props }">
              <v-card v-bind="props" class="teamCard ma-2" rounded outlined elevation="4">   
                <v-fade-transition hide-on-leave="true">
                  <div class="card_reveal ma-12" v-if="isHovering" >
                      <v-img class="teamIconsSelected" src="../assets/sharon.png"> </v-img>
                      <div class="textTeam">
                          <h3 style="font-size: 100%; color: #2c2c2c;">Hello, I’m Sharon, and I took on the role of Engineering Lead on rswp’s board of trustees in 2023. </h3>
                        <br> 
                          <h3 style="font-size: 100%; color: #2c2c2c;">My responsibilities include working closely with rural schools and partners, offering them technical guidance to ensure they have access to clean and safe water.</h3>
                        <br>
                          <h3 style="font-size: 100%; color: #2c2c2c;">I hold a degree in Water Resources Engineering and am currently employed at ATRO E&M. I play an active role there in advancing Green Infrastructure solutions for effective stormwater management. </h3>                
                      </div>
                   </div>    
                  <div class="ma-12">
                    <v-img class="teamIcons" src="../assets/sharon.png"> </v-img>
                      <h2> sharon akech </h2>
                        <h3 style="font-size: 150%;" class="water">engineering lead</h3>    
                    </div> 
                </v-fade-transition>
              </v-card>
            </v-hover>

            <v-hover v-slot="{ isHovering, props }">
              <v-card v-bind="props" class="teamCard ma-2" rounded outlined elevation="4">   
                <v-fade-transition hide-on-leave="true">
                  <div class="card_reveal ma-12" v-if="isHovering" >
                      <v-img class="teamIconsSelected" src="../assets/isobel.png"> </v-img>  
                      <div class="textTeam">
                          <h3 style="font-size: 100%;">Hi I’m Isobel, and I joined the board of trustees as Fundraising and Communications Lead in 2023.</h3>
                          <br>
                          <h3 style="font-size: 100%;">My focus at the moment is building our brand and communications strategy – basically what we stand for and how we share this with people.</h3>
                        <br>  
                          <h3 style="font-size: 100%;">My background is in marketing, comms and brand management and for the last 5 years I’ve done this work at Save the Children.</h3>                
                      </div>
                  </div>    
                  <div class="ma-12">
                    <v-img class="teamIcons" src="../assets/isobel.png"> </v-img>
                      <h2> isobel stewart </h2>
                      <h3 style="font-size: 150%;" class="water">fundraising and communications lead</h3>    
                  </div> 
                </v-fade-transition>
              </v-card>
            </v-hover>

            <v-hover v-slot="{ isHovering, props }">
              <v-card v-bind="props" class="teamCard ma-2" rounded outlined elevation="4">   
                <v-fade-transition hide-on-leave="true">
                  <div class="card_reveal ma-6" v-if="isHovering" >
                      <v-img  class="teamIconsSelected" src="../assets/matt.png"> </v-img>
                    
                      <div class="textTeam"> 
                        <h3 style="font-size: 100%; color: #2c2c2c;">I’m Matt, I joined the board of trustees in 2022 and took over rswp’s financial planning, controlling and reporting. </h3>
                      <br>
                        <h3 style="font-size: 100%; color: #2c2c2c;">I work directly with local partners to understand their handling of finances, drive efficiencies in uses of funding, improve our processes and keep rswp accountable to its stakeholders.</h3>
                      <br>
                        <h3 style="font-size: 100%; color: #2c2c2c;">I trained as a Chartered Accountant (CA), and was an active member of the ICAEW’s London Student Society where I was Treasurer for a couple of years. </h3>                
                    </div>
                  </div>
                <div class="card_reveal ma-12">
                  <v-img  class="teamIcons" src="../assets/matt.png"> </v-img>
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

.container {

}

.teamCard{
  text-align: center;
  height: 500px; 
  width: 350px;
  align-content: center;
  color:white;
  border-radius: 10%;
  position: relative;
}

.box{
 position: relative;
}

.card_reveal {
  position: relative;
  text-align: center;
  color: white;
}

.teamIcons{
border-radius: 50%;
height: 250px;
width: 250px;
position: relative;
align-content: center;
align-items: center;
}

.textTeam{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  font-size: 100%; 
  color: #2c2c2c;
  width: 300px;
}

.teamIconsSelected{
border-radius: 50%;
height: 100%;
width: 100%;
position: relative;
align-content: center;
align-items: center;
opacity: 30%;
}

</style>
