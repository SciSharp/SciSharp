<template>
    <div class="slide pa-5 grey darken-4" id="footer">
        <v-layout column
                  text-xs-center
                  wrap
                  class="pb-5"
        >
            <v-flex>
                <v-layout row wrap mx-5>
                    <v-spacer></v-spacer>

                    <v-flex xs4 mx-5>
                        <p><a href="https://gitter.im/sci-sharp/community" target="_blank" class="white--text">Contact us</a></p>
                        <p><a href="https://github.com/SciSharp" target="_blank" class="white--text">SciSharp on Github</a></p>
                    </v-flex>

<!--                    <v-flex xs4 mx-5>-->
<!--                    </v-flex>-->

                    <v-spacer></v-spacer>
                </v-layout>
<!--                <v-btn-->
<!--                        flat large outline-->
<!--                        href="https://github.com/SciSharp/TensorFlow.NET"-->
<!--                        target="_blank"-->
<!--                        color="#3fc6ee"-->
<!--                >-->
<!--                    <v-layout row>-->

<!--                        <v-icon class="mr-2">fab fa-github</v-icon>-->

<!--                        <span class="mr-2">Github</span>-->
<!--                    </v-layout>-->
<!--                </v-btn>-->
            </v-flex>
            <v-flex my-3>
                <p class="body-1">Copyright (c) 2019 - The SciSharp Team</p>
                <p class="body-1 grey--text">Powered by Vue, Nuxt and Vuetify</p>
            </v-flex>
        </v-layout>

    </div>

</template>

<script>
    export default {
        name: "Footer"
    }
</script>

<style scoped>

</style>