<template>
    <div class="slide pa-5 bg2" id="neuralnetworknet">
        <v-layout column
                  text-xs-center
                  wrap
                  class="pb-5"
        >
            <v-flex xs12>
                <img
                        src="@/assets/neuralnetwork.net.svg"
                        class="mt-5 mb-0"
                        height="300"
                        alt="NumSharp"
                ></img>
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
                <v-btn
                        text large outlined
                        href="https://github.com/Sergio0694/NeuralNetwork.NET"
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
        name: "SlideNeuralNetworkNet"
    }
</script>

<style scoped>

</style>