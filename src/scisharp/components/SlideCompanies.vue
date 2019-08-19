<template>
    <div class="slide pa-5 bg2" id="numpynet">
        <v-layout column
                  text-center
                  wrap
                  my-5
                  class="pb-5"
        >

            <v-flex mb-3 mt-5>
                <p class="title font-weight-light mb-3 white--text">
                    Companies using SciSharp STACK
                </p>
            </v-flex>

            <v-flex mb-5>
                <v-layout row wrap mx-md-5 justify-center>

                    <v-flex xs12 sm6 md3 lg2>
                        <a href="https://microsoft.com/">
                            <v-img
                                    :src="require('@/assets/3rd_party_microsoft.svg')"
                                    class="mt-5 mb-0"
                                    contain
                                    height="100"
                                    max-height="100"
                                    alt="Microsoft"
                            ></v-img>
                        </a>
                    </v-flex>

                    <v-flex xs12 sm6 md3 lg2>
                        <a href="https://curiosity.ai/">
                            <v-img
                                    :src="require('@/assets/3rd_party_curiosity.ai.svg')"
                                    class="mt-5 mb-0"
                                    contain
                                    height="100"
                                    max-height="100"
                                    alt="curiosity.ai"
                            ></v-img>
                        </a>
                    </v-flex>

                    <v-flex xs12 sm6 md3 lg2>
                        <a href="https://www.lokad.com/">
                            <v-img
                                    :src="require('@/assets/3rd_party_lokad.svg')"
                                    class="mt-5 mb-0"
                                    contain
                                    height="100"
                                    max-height="100"
                                    alt="LOKAD"
                            ></v-img>
                        </a>
                    </v-flex>

                    <v-flex xs12 sm6 md3 lg2>
                        <a href="http://www.footprintmatcher.com/">
                            <v-img
                                    :src="require('@/assets/3rd_party_everspry.svg')"
                                    class="mt-5 mb-0"
                                    contain
                                    height="100"
                                    max-height="100"
                                    alt="EVERSPRY"
                            ></v-img>
                        </a>
                    </v-flex>
                </v-layout>
            </v-flex>

        </v-layout>

    </div>

</template>

<script>
    export default {
        name: "SlideNumSharp"
    }
</script>

<style scoped>

</style>