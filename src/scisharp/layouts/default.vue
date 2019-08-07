<template>
  <v-app dark color="violet">
    <v-navigation-drawer app clipped temporary v-model="drawer">
      <v-list v-for="item in navbar_libs">
        <v-list-item @click="on_navbar_click(item)">
          <v-list-item-title>
            {{item.name}}
          </v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar app :clipped-left="true" class="violet theme--dark" elevate-on-scroll id="top">
<!--        :class="{ [`elevation-${toolbar_elevation}`]: true }"-->
      <v-app-bar-nav-icon dark @click="drawer=!drawer"></v-app-bar-nav-icon>
      <v-toolbar-title class="headline" @click="$vuetify.goTo(0, options)" style="cursor: pointer;">
        <span>SciSharp</span>
        <span class="font-weight-light text-uppercase"> STACK</span>
      </v-toolbar-title>

      <v-spacer></v-spacer>
      
      <v-btn fab text dark style="width: 32px; height: 32px;" href="https://medium.com/scisharp" target="_blank">
        <v-icon small>fab fa-medium</v-icon>
      </v-btn>

      <v-btn fab text dark style="width: 32px; height: 32px;" href="https://www.facebook.com/scisharp.stack.9" target="_blank">
        <v-icon small>fab fa-facebook</v-icon>
      </v-btn>

      <v-btn fab text dark style="width: 32px; height: 32px;" href="https://twitter.com/ScisharpS" target="_blank">
        <v-icon small>fab fa-twitter</v-icon>
      </v-btn>

      <v-btn fab text dark style="width: 32px; height: 32px;" href="https://gitter.im/sci-sharp/community" target="_blank">
        <v-icon small>fab fa-gitter</v-icon>
      </v-btn>

      <v-btn fab text dark style="width: 32px; height: 32px;" href="https://github.com/SciSharp" target="_blank">
          <v-icon small >fab fa-github</v-icon>
      </v-btn>
    </v-app-bar>

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
        drawer:false,
        toolbar_elevation:0,
        options: { // scrolling options for the menu buttons
          duration: 300,
          offset: 0,
          easing: 'easeInOutCubic',
        },
        navbar_libs: [
            { id:'#top', name: 'SciSharp STACK'},
            { id:'#tfnet', name: 'TensorFlow.NET'},
            { id:'#numsharp', name: 'NumSharp'},
            { id:'#kerasnet', name: 'Keras.NET'},
            { id:'#numpynet', name: 'Numpy.NET'},
            { id:'#scisharpcube', name: 'SciSharp Cube'},
            { id:'#neuralnetworknet', name: 'NeuralNetwork.NET'},
            { id:'#incubator', name: 'Incubator'},
        ]
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
    methods: {
        on_navbar_click(item) {
            console.log({item})
            this.$vuetify.goTo(item.id, this.options);
            this.drawer=false;
        }
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