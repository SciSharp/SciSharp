<template>
  <v-container>
    <v-layout column
              text-xs-center
              wrap
    >
      <v-flex xs12>
        <img
                src="@/assets/scisharp.svg"
                class="mt-5 mb-2"
                height="300"
        ></img>
      </v-flex>

      <v-flex mb-5>
        <h2 class="display-1 font-weight-light mb-3 white--text">
          A .NET based Open Source Ecosystem for Data Science, Machine Learning and AI
        </h2>
        <p class="title font-weight-light mb-3 white--text">
          SciSharp STACK brings all major ML/AI Frameworks from Python to .NET Core
        </p>
      </v-flex>

      <v-flex mb-5 mt-5>
        <v-layout row fill-height justify-center>

          <div class="xs-2 ma-3">
            <v-card class="white--text" color="#865fc5">
              <v-card-title>
                <h2 class="font-weight-light text-xs-center">For .NET Developers</h2>
              </v-card-title>
              <v-card-text class="text-xs-left">
                .NET developers are most productive with the tools they know and love. SciSharp's mission is to make sure
                that they don't have to leave that behind when reaching for opportunities in Data Science Machine Learning and AI.
                The well established Python
                based Machine Learning ecosystem is not quite accessible to millions of .NET developers. We are effectively
                changing that.
              </v-card-text>
            </v-card>
          </div>

          <div class="xs-2 ma-3">
            <v-card class="white--text" color="#865fc5">
              <v-card-title>
                <h2 class="font-weight-light text-xs-center">Cutting Edge Technology</h2>
              </v-card-title>
              <v-card-text class="text-xs-left">
                SciSharp provides ports and bindings to cutting edge Machine Learning frameworks like TensorFlow,
                Keras, PyTorch, Numpy and many more in .NET Core. Since the APIs of the ported libraries are so similar
                to the originals you can easily re-use all existing resources, documentation and community solutions to
                common problems in C# without much effort.
              </v-card-text>
            </v-card>
          </div>

          <div class="xs-2 ma-3">
            <v-card class="white--text" color="#865fc5">
              <v-card-title>
                <h2 class="font-weight-light text-xs-center">Cross-Platform</h2>
              </v-card-title>
              <v-card-text class="text-xs-left">
                All libraries of the SciSharp STACK target the cross-platform .NET Standard or .NET Core frameworks, which makes them
                usable on any major platform that supports .NET Core. We provide a ready-made Docker image with Jupyter Notebook
                being able to execute C# expressions and enabling you to start playing around with our libraries immediately.
              </v-card-text>
            </v-card>
          </div>

          <div class="xs-2 ma-3">
            <v-card class="white--text" color="#865fc5">
              <v-card-title>
                <h2 class="font-weight-light text-xs-center">Open Source</h2>
              </v-card-title>
              <v-card-text class="text-xs-left">
                SciSharp libraries are licensed under permissive licences, such as the Apache 2.0 license, allowing you to use them for any purpose
                including commercial applications as long as the copyright of the authors is retained. The Open Source
                nature of the SciSharp STACK is attracting many contributors who further extend and improve our efforts.
              </v-card-text>
            </v-card>
          </div>

        </v-layout>
      </v-flex>

    </v-layout>
  </v-container>
</template>

<script>
  export default {
    data: () => ({
    })
  }
</script>


<script>
// import Logo from '~/components/Logo.vue'
// import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {
    // Logo,
    // VuetifyLogo
  }
}
</script>
