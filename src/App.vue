<template style="main">

<header class="header-bar justify-end">
  <div class="header-content">
    <a 
      href="https://rswp.beehiiv.com/" 
      target="_blank"
      class="header-text"
    >
      join our newsletter →
    </a>
  </div>
</header>

<main>

  <Hero></Hero>

  <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

  <rss></rss>

  <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

  <rainwater></rainwater>

  <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
  <!-- 
  <story></story>

  <v-divider class="ma-10" style="opacity: 0%;" ></v-divider>
  -->
  <team></team>

  <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>
  <!-- 
  <newsletter></newsletter>

  <v-divider class="ma-10" style="opacity: 0%;" ></v-divider>
  -->
  <give></give>

  <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

  <foot></foot>

</main>

</template>

<script setup>
import Hero from "./components/Hero.vue"
import foot from "./components/footer.vue"
import story from "./components/Story.vue"
import newsletter from "./components/Newsletter.vue"
import team from "./components/Team.vue"
import rss from './components/rss.vue';
import rainwater from "./components/Rainwater.vue"
</script>

<script>
  export default {
    name: 'App',
    components: {
      rss
    }
  };
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

/* Sticky header styles */
.header-bar {
  position: fixed;
  height: 35px;
  top: 0;
  left: 0;
  right: 0;
  background-color: rgba(44, 44, 44, 1);
  color: #fff;
  padding: 10px 20px;
  z-index: 1000;
  display: flex;
  align-items: center;
}

.header-text {
  color: white;
  display: inline;
  font-size: 13px;
}

.header-text:hover {
  color: rgb(129, 221, 255);
}

.highlight {
  background-color: rgba(0, 174, 239, 0.8);
  font-family: ProximaNova-Bold;
  color: white;
}

/* Add margin to the main content to avoid overlap */
main {
  margin-top: 35px; /* Adjust this value based on your header's height */
  background: rgba(0,0,0,0) 0%;
}

.size {
    max-width: 80%;
    justify-content: center;
    background: rgba(44, 44, 44, 0.0);
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
  text-align: justify;
}

ul {
  margin: 0;
  font-family: ProximaNova-Regular;
  color: #2c2c2c;
}

a {
  font-family: ProximaNova-Regular;
  text-decoration: none;
  color: inherit;
}

</style>