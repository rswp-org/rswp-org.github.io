<template>
    <footer style="height: 350px;" >
        <v-col cols="6" max-width="1000px" class="ma-4">
          
            <v-row width="150px">
                <h1 style="color: white;">rural schools water project</h1>               
            </v-row>

            <v-row>
                <h3 style="color: white;">registered charity in england and wales number: 1170858</h3>
            </v-row>

            <v-row>
              <a href = "hello@rwsp.org">hello@rswp.org</a>
            </v-row>

            <v-row>
              <v-col align-self="start" align-start justify="start" cols="2">
                <v-img src="../assets/static/RSWP_Logo_Webicon_Blue.png"> </v-img>
              </v-col>
            </v-row>

        </v-col>
        <v-col style="align-items: end;" cols="4" >
          <v-row>
            <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.6.1/css/all.css">
            <v-col>

              <v-row class="mb-2">
                <a href="github.com"><i class="fab fa-github" style='scale: 100px;'></i></a>
              </v-row>
                <v-row class="mb-2"><p>Connect with us on Github!</p></v-row>
              

              <v-row class="mb-2">
                <a href="github.com"><i class="fab fa-linkedin" style='scale: 100px;'></i></a>
              </v-row>
              <v-row class="mb-2"><p>Connect with us on LinkedIn!</p></v-row>
           
            </v-col>
                   
    
          </v-row>
        </v-col>
        
    </footer>
</template>


<style scoped>

footer {
  align-items: center;
  background-color: #00aeef;
  border-radius: 0.1rem 0.1rem 0rem 0rem;
  color: white;
  display: flex;
  flex-wrap: nowrap;
  justify-content: space-between;
  padding: 3.75rem;
}

footer li.icon {
  display: inline-flex;
  font-size: 2rem;
  padding: 2.5rem;
}
</style>