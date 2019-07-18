<template>
    <div class="slide pa-5 bg1">
        <v-layout column
                  text-xs-center
                  wrap
                  class="pb-5"
        >
            <v-flex xs12>
                <img
                        src="@/assets/keras.net.svg"
                        class="mt-5 mb-0"
                        height="300"
                        alt="TensorFlow.NET"
                ></img>
            </v-flex>

            <v-flex mb-3>
                <h2 class="display-1 font-weight-light mb-3 white--text">
                    .NET bindings for Keras, the high-level Neural Network API for TensorFlow, CNTK and Theano
                </h2>
                <p class="title font-weight-light mb-3 white--text">
                    An easy-to-use Tool for Deep Learning
                </p>
            </v-flex>

            <v-flex>
                <v-btn
                        flat large outline
                        href="https://github.com/SciSharp/Keras.NET"
                        target="_blank"
                        color="#3fc6ee"
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
        name: "KerasNet"
    }
</script>

<style scoped>

</style>