<template>

  <Hero></Hero>

<v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

<give></give>

<v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

  <story></story>

  <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

  <team></team>

  <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

  <newsletter></newsletter>

  <v-divider class="ma-16" style="opacity: 0%;" ></v-divider>

  <foot></foot>

</template>

<script setup>
import Hero from "./components/Hero.vue"
import foot from "./components/footer.vue"
import story from "./components/Story.vue"
import newsletter from "./components/Newsletter.vue"
import team from "./components/Team.vue"
</script>