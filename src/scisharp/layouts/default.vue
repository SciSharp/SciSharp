<template>
  <v-app dark color="violet">
    <v-toolbar app class="violet elevation-0 theme--dark" >
      <v-toolbar-title class="headline">
        <v-layout row>
          <img class="mr-2"
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
      <v-btn
              flat
              href="https://github.com/SciSharp"
              target="_blank"
              class="theme--dark"
      >
        <v-layout row>

          <img class="mr-2"
                 src="@/assets/github_cat_white.svg"
                 style="width: 20px; height: 20px;"
          ></img>

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
</style>