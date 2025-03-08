<template>

<v-container class="rss-card">
  <v-card elevation="0">
    <v-row class="justify-center align-center">
      <h1>from the blog</h1>
    </v-row>
    <v-row class="justify-center align-center">
      <v-col cols="12" md="10" class="text-center">
        <p class="mt-0 mb-12" style="text-align: center;">our latest news and articles</p>
      </v-col>
    </v-row>
    <div class="rss-feed">
    <v-row style="column-gap: 16px" v-if="feedItems.length" dense>
      <!-- Loop through the first 3 articles -->
      <v-col v-for="(item, index) in feedItems.slice(0, 3)" :key="index" cols="12" md="4">
        <v-card max-height="300px" rounded @click="navigateToLink(item.link)">
          <!-- <v-img :src="item.thumbnail" height="100px" class="image-style"></v-img>-->
          <v-row class="ma-2 card-content">
            <p class="pa-0" style="font-size: 14px; text-align: left" v-if="item.pubDate">
              <span class="highlight">{{ formatDate(item.pubDate) }}</span>
              <span v-if="item.author" style="margin: 0 12px;">|</span>
              <span v-if="item.author">{{ item.author }}</span>
            </p>
            <h3 class="pa-0 title-limited-lines" style="font-size: 20px; text-align: left" v-text="item.title"></h3>
            <!-- <p class="pa-0" style="font-size: 14px" v-text="item.description"></p> -->
            <p class="pa-0 body-limited-lines" style="font-size: 15px; text-align: left;" v-if="item.content" v-text="getBodyText(item.content)"></p>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
    <p v-else>Loading articles...</p>
    </div>
  </v-card>
</v-container> 


  
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
    },
    formatDate(dateStr) {
    const date = new Date(dateStr);
    const options = { month: 'short', day: '2-digit', year: 'numeric' };
    return date.toLocaleDateString('en-US', options);
  },
  getBodyText(htmlContent) {
      // Create a temporary element to parse the HTML
      const tempDiv = document.createElement('div');
      tempDiv.innerHTML = htmlContent;
      // Find the div with the class "beehiiv__body"
      const beehiivBody = tempDiv.querySelector('.beehiiv__body');
      if (beehiivBody) {
        // Return the text content trimmed; you can also limit the length if needed
        return beehiivBody.textContent.trim();
      }
      return "";
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

.rss-card {
    max-width: 80%;
    padding: 0%;
    justify-content: center;
}

.card-content {
  display: flex;
  flex-direction: column; /* This stacks children vertically */
  gap: 16px; /* Adjust this value to control vertical spacing */
  align-items: left;
}

.title-limited-lines {
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
  overflow: hidden;
  text-overflow: ellipsis;
}

.body-limited-lines {
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  overflow: hidden;
  text-overflow: ellipsis;
}

.rss-feed .v-card {
  box-shadow: none; /* Removes the card's outline and shadow */
  border: none; /* Removes the border */
  background: rgba(44, 44, 44, 0.0); /* No background for the card */
  cursor: pointer; /* Make card clickable */
}

.rss-feed {
  padding: 0px;
  background: #ffffff;
  border-radius: 5px;
  margin: 0 auto;
  max-width: 98%;
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
  transform: scale(1.02);
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
  text-align: left;
  font-family: ProximaNova-Bold;
  color: #333;
}

/* Custom image styling */
.image-style {
  object-fit: cover;
  height: 200px;
}
</style>
