<template>
    <v-container class="page-banner" justify="center" fluid>
        <h1 style="justify-content: center; text-align: center;">how we work</h1> 

            <v-carousel hide-delimiters :show-arrows="false" cycle>

                <v-carousel-item class="card_content">
                    <v-img style="width: 100%; object-fit: cover;" src="../assets/ourwork1.jpg"> </v-img>
                    <div class="text-cont">
                        <h2 style="color: white;">🤝 local</h2>      
                        <h3 style="color: white;">Local organisations understand best what their communities need. We work with them to secure funding, provide operational support and enable long term learning.</h3>      
                    </div>
                </v-carousel-item>
            </v-carousel>
        
    </v-container>
</template>

<style scoped>
.card_content {
    max-width: 1400px;
    position: relative;
    text-align: center;
}

.caro-content{
    align-content: center;
    height: 100%;
    width: 100%; 
}

.caro-content img{
    align-content: center;
    height: 100%;
    width: 100%; 
}

.page-banner {
    max-width: 1400px;
}

.text-cont{
  position: absolute;
  bottom: 20px;
  right: 20px;
  background: linear-gradient(
    to top,
    rgba(0, 0, 0, 0.85),
    transparent
  );
  color: white;
  padding-left: 20px;
  padding-right: 20px;
}

</style>