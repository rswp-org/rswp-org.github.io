<template>

<Hero></Hero>

<v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

<story></story>

<v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

<v-container class="size">
  <v-card style="background: #00aeef;">
    <v-col class="d-flex flex-column justify-center align-center">
      <h2 class="py-2">stay in the know</h2>
      <h5>subscribe to our newsletter for all the latest updates and insights</h5>
      
        <v-row class="mt-5 mb-2"  justify="center">
          <v-card style="background: #00aeef">
          <iframe src="https://embeds.beehiiv.com/c613290e-b178-4159-a94b-037745d9ab4b?slim=true" data-test-id="beehiiv-embed" height="50" frameborder="0" scrolling="no" style="background: #00aeef"></iframe>
          </v-card>
        </v-row>

    </v-col>
  </v-card>
</v-container>

  <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

<foot></foot>

</template>

<script setup>
import Hero from "./components/Hero.vue"
import foot from "./components/footer.vue"
import story from "./components/Story.vue"
</script>


<style scoped>

.size {
  max-width: 80%;
  justify-content: center;
}

.beehiv {
  max-width: 80%;
  color: blue;
  justify-content: center;
  align-content: center;
  position: relative;

}

</style>

