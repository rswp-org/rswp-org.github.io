<template>
    <v-app>
      <v-main>
        <nav height="50" float>
            <v-container fluid>
                <v-row align="start">
                    <v-col align="center" height="50" class="logo" align-start>
                        <v-img height="100%" width="100%" src="./assets/RSWP_Logo_Vertical_FullColour.png"></v-img>
                    </v-col> 
                </v-row>
            </v-container>
        </nav>
        
 
        <v-container fluid >
                <v-row justify="center">
                    <v-col justify="center">
                    <h1 align="center">local, sustainable water services for primary schools in rural Uganda</h1>
                    </v-col>
                </v-row>
        </v-container>


        <v-container ma-4 justify="center" fluid>
            <v-row  justify="center">
            <h2>Join our mailing list!</h2>
            </v-row>

            <v-row justify="center" align="center">
                    <iframe src="https://embeds.beehiiv.com/c613290e-b178-4159-a94b-037745d9ab4b?slim=true" data-test-id="beehiiv-embed" height="52" frameborder="0" scrolling="no" style="margin: 0; border-radius: 0px !important; background-color: transparent;"></iframe>
                <!--<div class="button">
                    <a href="https://donate.stripe.com/8wM7tQ2oR2SI1So9AE" aria-label="donate to rswp" target="_blank" rel="noopener noreferrer">
                    <button>
                            <h2>donate</h2>
                            <div class="img">
                                <i class="bi bi-arrow-right-short" style="color:white"></i>
                            </div>
                    </button>
                    </a>
                    <a href="/donate"><p>more donation options</p></a>
                -->
            </v-row>
        </v-container>


        <Work></Work>


    </v-main>
  </v-app>
  </template>
  
  <script setup lang="ts">
    import Work from './components/ourWork.vue'

    //
  </script>
  
  <style>
  @font-face { 
  font-family: 'ProximaNova-Regular'; 
  src: url('/ProximaNova-Regular.otf') format('opentype'); 
} 
@font-face { 
  font-family: 'ProximaNova-Bold'; 
  src: url(/ProximaNova-Bold.otf) format('opentype');
}
@font-face { 
  font-family: 'ProximaNova-Black'; 
  src: url(/ProximaNova-Black.otf) format('opentype');}
html {
  background-color: white;
  color: #2c2c2c;
  font-family: 'ProximaNova-Regular';
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  overflow-x: hidden;
} 
body {
  line-height: 1.5;
  margin: 0;
  min-height: 100vh;
}
.leader {
  padding: 8rem;
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
.img {
  align-items: center;
  display: flex;
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
#menu-input{
  display: none;
}
#sidebar-menu li {
  text-align: center;
  padding: 2rem;
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
#kebab-menu {
  align-items: center;
  font-size: 5rem;
  right: 2rem;
  will-change: none;
}
#kebab-menu #sidebar-menu {
  background-color: white;
  box-sizing: border-box;
  color: #00aeef;
  height: 100%;
  left: -100vw;
  opacity: 0.95;
  position: fixed;
  padding: 8rem;
  top: 0;
  transition: 0.3s;
  visibility: hidden;
  width: 100%;
}
@media screen and (min-width: 1000px) {
  #sidebar-menu {
    font-size: 1.5rem;
  }
}
#menu-input:checked + #kebab-menu #sidebar-menu {
  visibility: visible;
  left: 0;
}
#menu-input:checked ~ .overlay{
 visibility: visible;
}
button {
  align-items: center;
  background-color: #00aeef;
  border: #00aeef;
  border-radius: 1rem;
  color: white;
  display: flex;
  font-weight: bold;
  justify-content: space-evenly;
  padding: 1.25rem 2rem; 
  margin: 2rem;
  min-width: 15rem;
}
button:hover {
  cursor: pointer;
  filter: brightness(85%);
}
.button {
  align-items: center;
  display: flex;
  justify-content: center;
  font-size: 1.5rem;
  margin: 5vh;
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

footer li.icon {
  display: inline-flex;
  font-size: 2rem;
  padding: 2.5rem;
}
img {
  border-radius: 50%;
  max-height: 20rem;
}
.img {
  align-items: center;
  display: flex;
  justify-content: flex-start;
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
  margin: 0;
  font-family: ProximaNova-Black;
  font-size: 4rem;
}
h2,h3,h4,h5,h6 {
  margin: 0;
  font-family: ProximaNova-Bold;
  font-size: 2rem;
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