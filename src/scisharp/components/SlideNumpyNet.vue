<template>
    <div class="slide pa-5 bg2" id="numpynet">
        <v-layout column
                  text-center
                  wrap
                  class="pb-5"
        >
            <v-flex xs12>
                <v-img
                        :src="require('@/assets/numpy.net.logo.svg')"
                        class="mt-5 mb-0"
                        contain
                        height="300"
                        max-height="300"
                        alt="Numpy.NET"
                ></v-img>
            </v-flex>

            <v-flex mb-3>
                <h2 class="display-1 font-weight-light mb-3 white--text">
                    The most complete .NET bindings for NumPy
                </h2>
                <p class="title font-weight-light mb-3 white--text">
                    A fundamental library for Scientific Computing, Machine Learning and AI
                </p>
            </v-flex>

            <v-flex>
                <v-btn large dark color="#661f76" href="https://github.com/SciSharp/Numpy.NET" target="_blank">
                    <v-layout row>
                        <v-icon class="mx-2" small>fab fa-github</v-icon>
                        <span class="mr-2">Github</span>
                    </v-layout>
                </v-btn>

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