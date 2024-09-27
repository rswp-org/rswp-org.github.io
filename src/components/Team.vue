<template>

    <v-container class="size">
        <v-card style="background: #00aeef; opacity: 1000%">
            <v-row class="justify-center align-center">
                <h2 class="py-2">meet the team</h2>
            </v-row>
            <v-row class="justify-center align-center">
                <h5 class="py-2">RSWP is run by an international team. We have a board of trustees...</h5>
            </v-row>
            <v-row class="py-2 justify-center align-center">
                <v-btn color="#033" rounded>Learn more about the team</v-btn>
            </v-row>
            <v-row class="d-flex justify-center">
                <v-col cols="12" md="6" lg="6" class="pa-4">
                <v-card class="pa-4">
                    <v-row cols="2">
                    <v-col class="d-flex justify-center align-center">
                        <v-img 
                        src="../assets/sharon_francis.JPG" 
                        class="rounded-lg" 
                        cover 
                        max-height="100%" 
                        max-width="100%" 
                        style="width: 150px; height: 150px;">
                        </v-img>
                    </v-col>
                    <v-col class="d-flex flex-column justify-center align-center">
                        <h4 class="text-center">Will Knapman</h4>
                        <h5 class="text-center">Founder and Operations Lead</h5>
                    </v-col>
                    </v-row>
                </v-card>
                </v-col>

                <v-col cols="12" md="6" lg="6" class="pa-4">
                <v-card class="pa-4">
                    <v-row cols="2">
                    <v-col class="d-flex justify-center align-center">
                        <v-img 
                        src="../assets/another_profile_image.JPG" 
                        class="circle" 
                        cover 
                        max-height="100%" 
                        max-width="100%" 
                        style="width: 150px; height: 150px;">
                        </v-img>
                    </v-col>
                    <v-col class="d-flex flex-column justify-center align-center">
                        <h4 class="text-center">Another Member</h4>
                        <h5 class="text-center">Another Role</h5>
                    </v-col>
                    </v-row>
                </v-card>
                </v-col>
            </v-row>
        </v-card>
    </v-container>

</template>

<style scoped>

    .size {
        max-width: 80%;
        justify-content: center;
        }

</style>