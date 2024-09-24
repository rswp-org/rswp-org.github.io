<template>
    <v-container class="size">
        <v-row cols="2">
            <v-col style="max-width: 35%" class="pa-6 mr-2">
                <v-card style="background: #00aeef;">
                    <v-col class="d-flex flex-column justify-center align-center">
                        <v-tabs v-model="tab" fixed-tabs="true">
                            <v-tab value="one-off">one-off</v-tab>
                            <v-tab value="monthly">monthly</v-tab>
                        </v-tabs>
                        <v-card-text>
                            <v-tabs-window v-model="tab">
                                <v-tabs-window-item value="one-off">
                                
                                </v-tabs-window-item>
                                <v-tabs-window-item value="one-off">
                                Now you see me 
                                </v-tabs-window-item>
                            </v-tabs-window>
                        </v-card-text>
                    </v-col>
                </v-card>
            </v-col>
        </v-row>
    </v-container>
</template>