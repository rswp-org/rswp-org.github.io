<template>
<v-container justify="center" fluid>
    <v-row justify="center">
        <h2 align="center">how we work</h2>
    </v-row>
    <v-row justify="center">
        <v-col align="center" justify="center">
            <v-card  max-height="500" max-width="900">
                <v-carousel rounded hide-delimiters align="center">
                    <v-hover v-slot="{ isHovering, props }">
                        <v-carousel-item width="1200" rounded v-bind="props">
                            <h2>🤝 local</h2>
                            <v-fade-transition>
                                <div v-if="isHovering">
                                    <h5>Local organisations understand best what their communities need. We work with them to secure funding, provide operational support and enable long term learning.</h5>
                                </div>
                            </v-fade-transition>
                        </v-carousel-item>
                    </v-hover>

                    <v-hover v-slot="{ isHovering, props }">
                        <v-carousel-item rounded v-bind="props">
                            <h2>🔁 sustainable</h2>
                            <v-fade-transition>
                                <div v-if="isHovering">
                                    <h5>Sustainability is vital for water services! We aspire to solutions that are reliable, affordable, well-managed and environmentally efficient.</h5>
                                </div>
                            </v-fade-transition>
                        </v-carousel-item>
                    </v-hover>
                    
                    <v-hover v-slot="{ isHovering, props }">
                        <v-carousel-item rounded v-bind="props">
                                    <h2>📈 data</h2>
                                    <v-fade-transition>
                                        <div v-if="isHovering">
                                            <h5>Local organisations understand best what their communities need. We work with them to secure funding, provide operational support and enable long term learning.</h5>
                                        </div>
                                    </v-fade-transition>
                            
                        </v-carousel-item>
                    </v-hover>

                </v-carousel>
            </v-card>
        </v-col>
    </v-row>
</v-container>
</template>