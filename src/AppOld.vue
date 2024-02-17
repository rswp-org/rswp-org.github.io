<template>
  <v-app>
    <v-main>

      <div class="banner">
        <!-- {{ $icon := resources.Get "images/RSWP_Logo_Vertical_FullColour.png" }}
        {{ with $icon }}
        <img class="logo" src="{{ $icon.RelPermalink }}">
        {{ end }} -->
        <h1 class="center-text">RSWP</h1>
    </div>
    
    <div style="margin-top: 50px;">
        <h2>Join our mailing list!</h2>
            <div align="center">
                <iframe src="https://embeds.beehiiv.com/c613290e-b178-4159-a94b-037745d9ab4b?slim=true" data-test-id="beehiiv-embed" height="52" frameborder="0" scrolling="no" style="margin: 0; border-radius: 0px !important; background-color: transparent;"></iframe>
            </div>
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
        </div>

      <div class="container">
          <h2 class="center-text">how we work</h2>
          <div class="row">
              <div class="col">
                  <div class="card">
                      <div class="card-body">
                          <h2>🤝 local</h2>
                          <p>Local organisations understand best what their communities need. We work with them to secure funding, provide operational support and enable long term learning.</p>
                      </div>
                  </div>
              </div>
              <div class="col">
                  <div class="card">
                      <div class="card-body">
                          <h2>🔁 sustainable</h2>
                          <p>Sustainability is vital for water services! We aspire to solutions that are reliable, affordable, well-managed and environmentally efficient.</p>
                      </div>
                  </div>
              </div>
              <div class="col">
                  <div class="card">
                      <div class="card-body">
                          <h2>📈 data</h2>
                          <p>We use data to understand what communities need, measure our own impact, and learn how we can do better next time.</p>
                      </div>
                  </div>
              </div>
          </div>
      </div>
  </v-main>
</v-app>
</template>

<script setup lang="ts">
  //
</script>

<style>


</style>