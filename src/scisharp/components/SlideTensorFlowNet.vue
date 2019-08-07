<template>
    <div class="slide pa-5 bg1" id="tfnet">
        <v-layout column
                  text-center
                  wrap
                  class="pb-5"
        >
            <v-flex xs12>
                <v-img
                        :src="require('@/assets/tf.net.logo.svg')"
                        class="mt-5 mb-0"
                        contain
                        height="300"
                        max-height="300"
                        alt="TensorFlow.NET"
                ></v-img>
            </v-flex>

            <v-flex mb-3>
                <h2 class="display-1 font-weight-light mb-3 white--text">
                    .NET Standard bindings for TensorFlow
                </h2>
                <p class="title font-weight-light mb-3 white--text">
                    Create, train and deploy Machine Learning models in C# or F#
                </p>
            </v-flex>

            <v-flex>
                <v-btn large dark color="#865fc5" href="https://github.com/SciSharp/TensorFlow.NET" target="_blank">
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
        name: "SlideTensorFlowNet"
    }
</script>

<style scoped>

</style>