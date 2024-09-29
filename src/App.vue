<template style="main">

  <Hero></Hero>

  <v-divider class="ma-10" style="opacity: 0%;" ></v-divider>

  <story></story>

  <v-divider class="ma-10" style="opacity: 0%;" ></v-divider>

  <team></team>

  <v-divider class="ma-10" style="opacity: 0%;" ></v-divider>

  <newsletter></newsletter>

  <v-divider class="ma-10" style="opacity: 0%;" ></v-divider>

  <give></give>

  <foot></foot>

</template>

<script setup>
import Hero from "./components/Hero.vue"
import foot from "./components/footer.vue"
import story from "./components/Story.vue"
import newsletter from "./components/Newsletter.vue"
import team from "./components/Team.vue"
</script>

<style>
@font-face { 
  font-family: 'ProximaNova-Regular'; 
  src: url('./assets/fonts/ProximaNova-Regular.otf') format('opentype'); 
  color: #2c2c2c;
} 
@font-face { 
  font-family: 'ProximaNova-Bold'; 
  src: url('./assets/fonts/ProximaNova-Bold.otf') format('opentype');
  color: #2c2c2c;
}
@font-face { 
  font-family: 'ProximaNova-Black'; 
  src: url('./assets/fonts/ProximaNova-Black.otf') format('opentype');
  color: #2c2c2c;
}

h1 {
  margin: 0;
  font-family: ProximaNova-Black;
  color: #00aeef;
}

h2 {
  margin: 0;
  font-family: ProximaNova-Black;
  color: #2c2c2c;
}

h5 {
  margin: 0;
  font-family: ProximaNova-Bold;
  color: #00aeef;
}

h4 {
  margin: 0;
  font-family: ProximaNova-Bold;
  color: #00aeef;
}

h3,h6 {
  margin: 0;
  font-family: ProximaNova-Bold;
  color: #2c2c2c;
}

p {
  margin: 0;
  font-family: ProximaNova-Regular;
  color: #2c2c2c;
}

a {
  text-decoration: none;
  color: inherit;
}

main{
  background: rgb(0,0,0);
background: linear-gradient(90deg, rgba(0,0,0,0) 0%, rgba(0,174,239,0.08167016806722693) 63%, rgba(0,174,239,1) 100%);
}

</style>