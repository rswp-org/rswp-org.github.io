<template>
  <div class="rss-feed">
    <h1>Read Our Latest Work</h1>
    <v-row v-if="feedItems.length" dense>
      <!-- Loop through the first 3 articles -->
      <v-col v-for="(item, index) in feedItems.slice(0, 3)" :key="index" cols="12" sm="4">
        <v-card max-height="300px" rounded @click="navigateToLink(item.link)">
          <v-img :src="item.thumbnail" height="200px" class="image-style"></v-img>
          <v-row class="ma-2" align="center" justify="center">
            <h3 class="pa-0" v-text="item.title"></h3>
          </v-row>
        </v-card>
      </v-col>
    </v-row>

    <p v-else>Loading articles...</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      feedItems: [],
      loading: true,
      error: null
    };
  },
  mounted() {
    this.fetchRSSFeed();
  },
  methods: {
    async fetchRSSFeed() {
      const feedUrl = 'https://rss.beehiiv.com/feeds/hHhwMc7G7A.xml';
      const apiUrl = `https://api.rss2json.com/v1/api.json?rss_url=${encodeURIComponent(feedUrl)}`;
     
      try {
        const response = await fetch(apiUrl);
        const data = await response.json();
        console.log(data)
       
        if (data.status === 'ok') {
          this.feedItems = data.items;
          this.loading = false;
        } else {
          this.error = 'Failed to load RSS feed';
          this.loading = false;
        }
      } catch (err) {
        this.error = 'An error occurred while fetching the RSS feed';
        this.loading = false;
      }
    },
    navigateToLink(url) {
      window.open(url, '_blank');
    }
  }
};
</script>

<style scoped>
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
  color: #00aeef;
}

h4 {
  margin: 0;
  font-family: ProximaNova-Bold;
  color: #00aeef;
}

.rss-feed .v-card {
  box-shadow: none; /* Removes the card's outline and shadow */
  border: none; /* Removes the border */
  background: none; /* No background for the card */
  cursor: pointer; /* Make card clickable */
}

.rss-feed {
  padding: 20px;
  background: #ffffff;
  border-radius: 5px;
  margin: 0 auto;
  max-width: 80%;
}

.rss-feed h2 {
  text-align: center;
  font-size: 1.5em;
}

.rss-feed .v-img {
  position: relative;
}

.rss-feed .v-img .v-container {
  background: rgba(0, 0, 0, 0.5); /* Darken the bottom of the image */
}

.rss-feed .v-row {
  padding: 0;
}

.rss-feed .v-col {
  padding: 10px;
}

.rss-feed .v-card:hover {
  transform: scale(1.05);
  transition: transform 0.3s ease;
}

.rss-feed .custom-card {
  max-width: 100%; /* Ensure card takes full width */
  height: 300px; /* Fixed height for the card */
  display: flex;
  flex-direction: column;
}

.rss-feed .custom-card .v-img {
  object-fit: cover; /* Ensures the image covers the space without stretching */
  height: 200px; /* Set a fixed height for images */
}

.rss-feed h3 {
  text-align: center;
  font-family: ProximaNova-Bold;
  color: #333;
}

/* Custom image styling */
.image-style {
  object-fit: cover;
  height: 200px;
}
</style>
