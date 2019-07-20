<template>
  <v-app dark color="violet">
    <v-toolbar app class="violet theme--dark" :class="{ [`elevation-${toolbar_elevation}`]: true }" ref="toolbar">
      <v-toolbar-title class="headline" @click="$vuetify.goTo(0, options)" style="cursor: pointer;">
        <v-layout row>
          <img class="mr-0"
                 src="@/assets/icon.svg"
                 contain
                 style="width: 48px; height: 48px;"
          ></img>
          <div class="my-2 ml-2">
            <span>SciSharp</span>
            <span class="font-weight-light text-uppercase"> STACK</span>
          </div>
        </v-layout>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-layout row>
        <v-btn flat dark @click="$vuetify.goTo('#tfnet', options)">TensorFlow.NET</v-btn>
        <v-btn flat dark @click="$vuetify.goTo('#numsharp', options)">NumSharp</v-btn>
        <v-btn flat dark @click="$vuetify.goTo('#kerasnet', options)">Keras.NET</v-btn>
        <v-btn flat dark @click="$vuetify.goTo('#numpynet', options)">Numpy.NET</v-btn>
        <v-btn flat dark @click="$vuetify.goTo('#scisharpcube', options)">SciSharp Cube</v-btn>
        <v-btn flat dark @click="$vuetify.goTo('#neuralnetworknet', options)">NeuralNetwork.NET</v-btn>
        <v-btn flat dark @click="$vuetify.goTo('#incubator', options)">Incubator</v-btn>
      </v-layout>
      <v-spacer></v-spacer>
      
      <v-btn fab flat dark style="width: 32px; height: 32px;" href="https://medium.com/scisharp" target="_blank">
        <v-icon small>fab fa-medium</v-icon>
      </v-btn>

      <v-btn fab flat dark style="width: 32px; height: 32px;" href="https://www.facebook.com/scisharp.stack.9" target="_blank">
        <v-icon small>fab fa-facebook</v-icon>
      </v-btn>

      <v-btn fab flat dark style="width: 32px; height: 32px;" href="https://twitter.com/ScisharpS" target="_blank">
        <v-icon small>fab fa-twitter</v-icon>
      </v-btn>

      <v-btn fab flat dark style="width: 32px; height: 32px;" href="https://gitter.im/sci-sharp/community" target="_blank">
        <v-icon small>fab fa-gitter</v-icon>
      </v-btn>

      <v-btn fab flat dark style="width: 32px; height: 32px;" href="https://github.com/SciSharp" target="_blank">
          <v-icon small >fab fa-github</v-icon>
      </v-btn>
    </v-toolbar>

    <v-content class="violet">
      <nuxt />
    </v-content>
  </v-app>
</template>

<script>
  export default {
    name: 'App',
    components: {
    },
    data () {
      return {
        options: { // scrolling options for the menu buttons
          duration: 300,
          offset: 0,
          easing: 'easeInOutCubic',
        },
        toolbar_elevation:0,
      }
    },
    mounted() {
      window.addEventListener("scroll", (ev)=> {
        var yoff=window.pageYOffset;
        console.log({yoff})
        if (!yoff || yoff==0)
          this.toolbar_elevation=0;
        else
          this.toolbar_elevation=1;
      })
    },
    methods() {

    },
  }
</script>

<style>
  .violet {
    background-color: #661f76 !important;
  }
  .bg1 {
    background-color: #661f76 !important;
  }
  .bg2 {
    background-color: #865fc5;
  }
  .bg3 {
    background-color: white;
  }
  .slide {
    width: 100%;
    margin-left: 0;
    margin-right: 0;
  }
</style>