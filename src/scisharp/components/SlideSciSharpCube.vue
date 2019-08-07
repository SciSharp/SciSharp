<template>
    <div class="slide pa-5 bg1" id="scisharpcube">
        <v-layout column
                  text-center
                  wrap
                  class="pb-5"
        >
            <v-flex xs12 my-5>
                <v-img
                        :src="require('@/assets/SciSharpCube.svg')"
                        class="mt-5 mb-0"
                        contain
                        height="300"
                        max-height="300"
                        alt="SciSharpCube"
                ></v-img>
            </v-flex>

            <v-flex mb-3>
                <h2 class="display-1 font-weight-light mb-3 white--text">
                    Experience all the latest features of SciSharp Machine Learning tools in a Docker container
                </h2>
                <p class="title font-weight-light mb-3 white--text">
                    Features a Jupyter Notebook presenting Demos of the SciSharp Libraries
                </p>
            </v-flex>

            <v-flex>
                <v-btn large dark color="#865fc5" href="https://github.com/SciSharp/SciSharpCube" target="_blank">
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
        name: "SlideSciSharpCube"
    }
</script>

<style scoped>

</style>