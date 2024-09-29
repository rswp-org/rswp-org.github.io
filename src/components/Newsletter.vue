<template>
    
    <v-container class="size">
    <v-card class="rounded-lg" style="background-color: rgba(0, 174, 239, 0.5);">
        <v-col class="d-flex flex-column justify-center align-center">
        <v-row>
            <img src="../assets/mail.svg" class="icon mx-1 py-1" style="width: 60px; height: 60px;"/>
        </v-row> 
        <v-row class="justify-center align-center">
            <v-col cols="12" md="10" class="text-center">
                <h1 class="py-2" style="color: black">stay in the know</h1>
                <p>subscribe to our newsletter for all the latest updates and insights</p>
            </v-col>
        </v-row>
            <v-row class="mt-5 mb-2"  justify="center">
            <v-card style="background: #00aeef">
            <iframe src="https://embeds.beehiiv.com/c613290e-b178-4159-a94b-037745d9ab4b?slim=true" data-test-id="beehiiv-embed" height="50" frameborder="0" scrolling="no" style="background: #00aeef"></iframe>
            </v-card>
            </v-row>

        </v-col>
    </v-card>
    </v-container>

</template>

<style scoped>

    .size {
    max-width: 80%;
    justify-content: center;
    }

    .beehiv {
    max-width: 80%;
    color: blue;
    justify-content: center;
    align-content: center;
    position: relative;

    }

</style>