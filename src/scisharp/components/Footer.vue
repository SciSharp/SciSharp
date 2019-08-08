<template>
    <div class="slide pa-5 grey darken-4" id="footer">
        <v-layout column
                  text-center
                  justify-center
                  wrap
                  class="pb-5"
        >
            <v-flex xs12 md6 >
                    <p><a href="https://gitter.im/sci-sharp/community" target="_blank" class="white--text">Contact us</a></p>
                    <p><a href="https://github.com/SciSharp" target="_blank" class="white--text">SciSharp on Github</a></p>
            </v-flex>
            <v-flex xs12 md6 my-3 >
                <p class="body-1 grey--text" ><small>Copyright (c) 2019 - The SciSharp Team</small></p>
                <p class="body-1 grey--text"><small>Powered by Vue, Nuxt and Vuetify</small></p>
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