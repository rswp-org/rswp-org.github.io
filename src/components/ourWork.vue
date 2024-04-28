<template>
    <v-container class="page-banner" justify="center" fluid>
        <h1 style="justify-content: center; text-align: center;">how we work</h1> 
    
            <v-carousel class="card_content" hide-delimiters :show-arrows="false" cycle>

                <v-carousel-item class="caro-content" >
                    <v-img style="width: 300px; height: 337px; object-fit: none;" width="100%" src="../assets/ourwork1.jpg"> <!--Get morgans help? Zoom in on hover-->
                        <div class="text-cont">
                            <h2 style="color: white;">🤝 local</h2>      
                            <h3 style="color: white;">Local organisations understand best what their communities need. We work with them to secure funding, provide operational support and enable long term learning.</h3>      
                        </div>
                    </v-img> 
                </v-carousel-item>

                <v-carousel-item class="caro-content" >
                    <v-img  src="../assets/test.jpg"> <!--Get morgans help? Zoom in on hover-->
                    <h2>🔁 sustainable</h2>
                    <h3>Sustainability is vital for water services! We aspire to solutions that are reliable, affordable, well-managed and environmentally efficient.</h3>
                    </v-img>  
                </v-carousel-item>
            
                <v-carousel-item class="caro-content" >
                    <v-img  src="../assets/ourwork1.jpg"> <!--Get morgans help? Zoom in on hover-->
                        <h2>📈 data</h2>
                        <h3>Local organisations understand best what their communities need. We work with them to secure funding, provide operational support and enable long term learning.</h3>
                    </v-img>  
                </v-carousel-item>
                   
                  
            </v-carousel>
        
    </v-container>
</template>

<style scoped>
.card_content {
    max-width: 1400px;
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
    align-items: start;
    background: linear-gradient(
    to top,
    rgba(0, 0, 0, 0.85),
    transparent
  );
}

</style>