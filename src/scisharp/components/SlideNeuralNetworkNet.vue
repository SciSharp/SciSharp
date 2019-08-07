<template>
    <div class="slide pa-5 bg2" id="neuralnetworknet">
        <v-layout column
                  text-center
                  wrap
                  class="pb-5"
        >
            <v-flex xs12 my-5 py-5>
                <v-img
                        :src="require('@/assets/neuralnetwork.net.svg')"
                        class="mt-5 mb-0"
                        contain
                        height="250"
                        max-height="250"
                        alt="NeuralNetwork.NET"
                ></v-img>
            </v-flex>

            <v-flex mb-3>
                <h2 class="display-1 font-weight-light mb-3 white--text">
                    A TensorFlow-inspired Neural Network Library built from Scratch
                </h2>
                <p class="title font-weight-light mb-3 white--text">
                    Written in C# 7.3 for .NET Standard 2.0, with GPU support through cuDNN
                </p>
            </v-flex>

            <v-flex>
                <v-btn large dark color="#661f76" href="https://github.com/Sergio0694/NeuralNetwork.NET" target="_blank">
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
        name: "SlideNeuralNetworkNet"
    }
</script>

<style scoped>

</style>