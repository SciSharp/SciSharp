<template>
    <div class="slide pa-5 bg2" id="numsharp">
        <v-layout column
                  text-center
                  wrap
                  class="pb-5"
        >
            <v-flex xs12>
                <v-img
                        :src="require('@/assets/numsharp.logo.svg')"
                        class="mt-5 mb-0"
                        contain
                        height="300"
                        max-height="300"
                        alt="NumSharp"
                ></v-img>
            </v-flex>

            <v-flex mb-3>
                <h2 class="display-1 font-weight-light mb-3 white--text">
                    A highly optimized pure C# port of NumPy
                </h2>
                <p class="title font-weight-light mb-3 white--text">
                    N-D Tensor Computation Library for Data Science, Machine Learning and AI
                </p>
            </v-flex>

            <v-flex>
                <v-btn large dark color="#661f76" href="https://github.com/SciSharp/NumSharp" target="_blank">
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