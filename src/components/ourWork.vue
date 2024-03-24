<template>
    <v-container style="max-width: 1400px; align-items: center;" class="page-banner" justify="center" fluid>
        <h1 style="justify-content: center; text-align: center;">how we work</h1> 
    
            <v-carousel class="card_content" hide-delimiters :show-arrows="false" cycle>

                        <v-carousel-item class="caro-content" >
                            <v-img src="../assets/ourwork1.jpg"> <!--Get morgans help? Zoom in on hover-->
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

}

.card_content{

}


.caro-content{
    align-content: center;
    
}

.page-banner {
    padding: 0;
    transition: transform .2s;
    z-index: 1;
}

.text-cont{
  bottom: 0;
  left: 0;
    background: linear-gradient(
    to top,
    rgba(0, 0, 0, 0.85),
    transparent
  );
}

</style>