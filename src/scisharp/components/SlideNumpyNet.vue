<template>
    <div class="slide pa-5 bg2" id="numpynet">
        <v-layout column
                  text-xs-center
                  wrap
                  class="pb-5"
        >
            <v-flex xs12>
                <img
                        src="@/assets/numpy.net.logo.svg"
                        class="mt-5 mb-0"
                        height="300"
                        alt="Numpy.NET"
                ></img>
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
                <v-btn
                        flat large outline
                        href="https://github.com/SciSharp/Numpy.NET"
                        target="_blank"
                        color="#3fc6ee"
                        style="background-color: #661f76 !important;"
                >
                    <v-layout row>

                        <v-icon class="mr-2">fab fa-github</v-icon>

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