<template>
    <v-app>
      <v-main>
            <v-container  class="mb-16, pa-8" style="max-width: 1100px; flex">
                <v-row align="start">

                    <v-col align="start" class="logo" align-start>
                        <v-img  rounded width="150px" src="./assets/RSWP_Logo_Horizontal_FullColour.png"></v-img>
                    </v-col> 

                    <v-spacer></v-spacer>
                      <v-col cols="2" align-self="end" justify="end">
                          <v-btn justify-end height="50" max-width="150" class="button" href="https://rswp.beehiiv.com/" color="primary">
                                  <p style="text-transform: unset !important;  font-size: 50%; color:white">newsletter</p>
                          </v-btn> 
                      </v-col>
                        <v-col cols="2" align-self="end">
                          <v-btn justify-end height="50" max-width="150" class="button" href="https://donate.stripe.com/8wM7tQ2oR2SI1So9AE" color="primary">
                                  <p style="text-transform: unset !important;  font-size: 50%; color:white">donate</p>
                          </v-btn>       
                        </v-col>
                    
                </v-row>
            </v-container>
        
            <v-divider class="ma-12" style="opacity: 0%;" ></v-divider>
 
        <v-container class="mt-16, pa-8" style="max-width: 1100px; flex">
     
                <v-row class="mb-8" justify="start">
                    <v-col class="mt-14" justify="start">

                      <h1 class="mb-10">data-driven <span style="color: #00aeef;">water</span> solutions for Ugandan schools</h1>

                        <p style="font-size: 100%;" class="mt-8" >If you wish to support us further please press the link below</p>

                        <v-btn width="200" height="50" class="button mt-8" href="https://donate.stripe.com/8wM7tQ2oR2SI1So9AE" color="primary">
                                  <h3 style="font-size: 100%; color:white">donate</h3>
                        </v-btn>

                    </v-col>
                    <v-col style="scale: 100%;" align-self="start">
                      <v-img style="min-height: 100px; text-align: left; display: block;" src="./assets/RSWP_Logo_Horizontal_FullColour.png"></v-img>
                    </v-col>
                </v-row>        
        </v-container>
        
        
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
        <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

        <!--NEWLETTER SECTION
        <v-container style="max-width: 1100px; ">
          <h2 style="text-align: start; color: black;">check out our latest newsletter articles!</h2>
          <v-card color="primary" elevation="4">
            
            <v-row class="ma-2" justify="center">
              <h3 style="text-align: start; color: white; padding-bottom: 10%;">latest Posts</h3>             
            </v-row>

              <v-row class="" justify="start" >
                <v-col class="" cols="3">
                
                  <v-card justify="center" class="ma-2" outlined  height="350px" width="250px" color="white" elevation="4" rounded>
                    <h4 style="text-align: center;">Post 1</h4>
                    <v-img :src=imageUrl></v-img>
                  </v-card>

                  </v-col>
                  <v-col class="mt-8" cols="3">
                  
                  <v-card justify="center" class="ma-2" outlined  height="350px" width="250px" color="white" elevation="4" rounded>
                    <h4 style="text-align: center;">Post 1</h4>
                    <v-img src="../assets/images/test.jpg"></v-img>
                  </v-card>
              </v-col>

              </v-row>
          </v-card>
        </v-container>
      -->
       

        <Work ></Work>

        <team></team>

        <Foot></Foot>

    </v-main>
  </v-app>
  </template>
  
  <script>
    import Work from './components/ourWork.vue';
    import signup from './components/signup.vue';
    import team from './components/team.vue';
    import Map from './components/Map.vue';
    import Foot from './components/footer.vue';
    import axios from 'axios';
    import { ref, onMounted } from 'vue';

    export default {
    name: 'App',
    channel: "",
    imageUrl: "",
    //const imageUrl = ref('');

      components: {
        Map,
        team,
        signup,
        Work,
        Foot,
        imageUrl: "",
      },

      onMounted() {
        axios.get('https://rss.beehiiv.com/feeds/hHhwMc7G7A.xml')
        .then(function (response) {
          const xmlString = response.data;
          console.log(xmlString) 

          const parser = new DOMParser();
          const xmlDoc = parser.parseFromString(xmlString, "text/xml");
        

          const channels = xmlDoc.getElementsByTagName('channel');

          // Iterate over each channel
          for (let i = 0; i < channels.length; i++) {
            const channel = channels[i];
            imageUrl = channel.getElementsByTagName('url')[i];
            console.log(imageUrl)
          }
        });
      }


    }
  
</script>


<style>
@font-face { 
  font-family: 'ProximaNova-Regular'; 
  src: url('./assets/ProximaNova-Regular.otf') format('opentype'); 
  color: #2c2c2c;
} 
@font-face { 
  font-family: 'ProximaNova-Bold'; 
  src: url('./assets/ProximaNova-Bold.otf') format('opentype');
  color: #2c2c2c;
}
@font-face { 
  font-family: 'ProximaNova-Black'; 
  src: url('./assets/ProximaNova-Black.otf') format('opentype');
  color: #2c2c2c;
}

body {
  line-height: 1.5;
  margin: 0;
  min-height: 100vh;
}

nav {
  align-items: baseline;
  background: white; 
  border-bottom: 0.1rem solid #2c2c2c20;
  box-shadow: 0.1rem 0.1rem #2c2c2c20;
  display: flex;
  justify-content: space-between;
  padding: 1.875rem;
  padding-bottom: 0rem;
  position: sticky;
  top: 0;
  
}
header {
  align-items: center;
  display: flex;
  flex-direction: column;
} 
.logo {
  max-width: 10rem;
  border-radius: 0;
}

.banner {
  align-items: center;
  display: flex;
  flex: 1 0 auto;
  flex-direction: column;
}
.center-text {
  text-align: center;
}

.overlay{
  background-color: white;
  left: 0;
  height: 100%;
  opacity: 0;
  overflow: hidden;
  top: 0;
  transition: opacity .35s, visibility .35s, height .35s;
  visibility: hidden;
  width: 100%;
  z-index: -1;
}

#menu-input:checked + #kebab-menu #sidebar-menu {
  visibility: visible;
  left: 0;
}
#menu-input:checked ~ .overlay{
 visibility: visible;
}
button {
  background-color: #00aeef;
  border: #00aeef;
  border-radius: 1rem;
  color: white;
  display: flex;
  min-width: 15rem;
  
}
button:hover {
  cursor: pointer;
  filter: brightness(85%);
}
.button {
  display: flex;
  font-size: 1.5rem;
  text-transform:lowercase
}
i {
  font-size: 3rem;
}
ul {
  font-family: 'ProximaNova-Bold';
  list-style: none;
}
a {
  color: currentColor;
  text-decoration: none;
}

em {
  color: #00aeef;
  font-style: normal;
}
form {
  display: flex;
  flex-direction: column;
  padding: 4rem;
}
label {
  font-size: 2em;
  font-family: ProximaNova-Bold;
}
input, select, textarea {
  border: 0.1rem solid rgba(0,0,0,0.2);
  font-size: 2em;
  padding: 1rem;
  margin-bottom: 1rem;
}
.row {
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  justify-content: space-evenly;
  margin: 2rem;
}
@media screen and (min-width: 1000px) {
  .row {
    flex-direction: row;
  }
}
.col {
  flex: 30%;
  margin: 1rem;
  margin-bottom: 2rem;
}
h1 {
  margin: -1;
  font-family: ProximaNova-Black;
  font-size: 2.75rem;
  text-align: left;
  letter-spacing: -2px;
  line-height: 120%;
  color: #2c2c2c;
}
.water {
  color: #00aeef;
}
h2,h3,h4,h5,h6 {
  margin: 0;
  font-family: ProximaNova-Bold;
  font-size: 2rem;
  color: #2c2c2c;
}
p {
  font-size: 1.5em;
}
.card {
  align-items: center;
  border: 0.1rem solid #2c2c2c20;
  border-radius: 1rem;
  box-shadow: 0.1rem 0.1rem  #2c2c2c20;
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  padding: 2rem;
}
.card-content {
  margin: 1rem;
}
#content {
  padding: 4rem
}



  </style>