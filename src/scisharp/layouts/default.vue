<template>
  <v-app dark color="violet">
    <v-toolbar app class="violet elevation-0 theme--dark" ref="toolbar">
      <v-toolbar-title class="headline">
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

      <v-btn
              flat
              href="https://github.com/SciSharp"
              target="_blank"
              class="theme--dark"
      >
        <v-layout row>

          <v-icon small class="mr-2">fab fa-github</v-icon>

          <span class="mr-2">Github</span>
        </v-layout>
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
        //
      }
    }
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