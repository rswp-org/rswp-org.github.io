<template>
  <div class="rss-feed">
    <h2>RSS Feed</h2>
    <ul v-if="feedItems.length">
      <li v-for="(item, index) in feedItems" :key="index">
        <a :href="item.link" target="_blank">{{ item.title }}</a>
        <p v-html="item.description"></p>
      </li>
    </ul>
    <p v-else>Loading feed</p>
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
    }
  }
};
</script>
 
<style scoped>
.rss-feed {
  padding: 20px;
  background: #f4f4f4;
  border-radius: 5px;
  max-width: 800px;
  margin: 0 auto;
}
 
.rss-feed h2 {
  text-align: center;
  font-size: 1.5em;
}
 
.rss-feed ul {
  list-style-type: none;
  padding: 0;
}
 
.rss-feed li {
  margin: 10px 0;
}
 
.rss-feed li a {
  font-weight: bold;
  color: #007BFF;
  text-decoration: none;
}
 
.rss-feed li a:hover {
  text-decoration: underline;
}
 
.rss-feed p {
  color: #555;
}
</style>