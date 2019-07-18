<template>
  <v-layout column id="hmm">

    <!--    main screen-->
    <div class="slide mt-5">
    <v-layout column
              text-xs-center
              wrap
    >
      <v-flex xs12>
        <img
                src="@/assets/scisharp-stack.svg"
                class="mt-5 mb-2"
                height="300"
                alt="SciSharp STACK"
        ></img>
      </v-flex>

      <v-flex mb-5>
        <h2 class="display-1 font-weight-light mb-3 white--text">
          A .NET based Open Source Ecosystem for Data Science, Machine Learning and AI
        </h2>
        <p class="title font-weight-light mb-3 white--text">
          SciSharp STACK brings all major ML/AI Frameworks from Python to .NET
        </p>
      </v-flex>
    </v-layout>
      <v-layout column
                text-xs-center
                wrap
                class="bg2"
                px-5
      >
      <v-flex mb-5 mt-5 pt-3>
        <v-layout row fill-height justify-center>

          <div class="xs-2 ma-3">
            <v-card light class="elevation-10">
              <v-card-title >
                <h2 class="text-xs-center">For .NET Developers</h2>
              </v-card-title>
              <v-card-text class="text-xs-left">
                .NET developers are most productive with the <b>tools they know and love</b>. SciSharp's mission is to make sure
                that they don't have to leave that behind when reaching for opportunities in Data Science Machine Learning and AI.
                The well established Python
                based Machine Learning ecosystem is not quite accessible to millions of .NET developers. We are effectively
                changing that.
              </v-card-text>
            </v-card>
          </div>

          <div class="xs-2 ma-3">
            <v-card light class="elevation-10">
              <v-card-title>
                <h2 class="text-xs-center">Cutting Edge Technology</h2>
              </v-card-title>
              <v-card-text class="text-xs-left">
                SciSharp provides ports and bindings to cutting edge Machine Learning frameworks like <b>TensorFlow</b>,
                <b>Keras</b>, <b>PyTorch</b>, <b>Numpy</b> and many more in .NET Core. Since the APIs of the ported libraries are so similar
                to the originals you can easily re-use all existing resources, documentation and community solutions to
                common problems in C# without much effort.
              </v-card-text>
            </v-card>
          </div>

          <div class="xs-2 ma-3">
            <v-card  light class="elevation-10">
              <v-card-title>
                <h2 class="text-xs-center">Cross-Platform</h2>
              </v-card-title>
              <v-card-text class="text-xs-left">
                All libraries of the SciSharp STACK target the cross-platform <b>.NET Standard Framework</b>, which makes them
                usable on any major platform that supports .NET Core. We provide a ready-made Docker image with Jupyter Notebook
                being able to execute C# expressions and enabling you to start playing around with our libraries immediately.
              </v-card-text>
            </v-card>
          </div>

          <div class="xs-2 ma-3">
            <v-card  light class="elevation-10">
              <v-card-title>
                <h2 class="text-xs-center">Open Source</h2>
              </v-card-title>
              <v-card-text class="text-xs-left">
                SciSharp libraries are licensed under permissive licences, such as the Apache 2.0 license, allowing you to use them for any purpose
                including <b>commercial applications</b> as long as the copyright of the authors is retained. The Open Source
                nature of the SciSharp STACK is attracting many contributors who further extend and improve it.
              </v-card-text>
            </v-card>
          </div>

        </v-layout>
      </v-flex>

    </v-layout>
  </div>

    <SlideTensorFlowNet></SlideTensorFlowNet>
    <SlideNumSharp></SlideNumSharp>
    <SlideKerasNet></SlideKerasNet>
    <SlideNumpyNet></SlideNumpyNet>
  </v-layout>
</template>

<script>
  export default {
    data: () => ({
    })
  }
</script>


<script>
 import SlideTensorFlowNet from '~/components/SlideTensorFlowNet.vue'
 import SlideNumSharp from '~/components/SlideNumSharp.vue'
 import SlideKerasNet from "~/components/SlideKerasNet";
 import SlideNumpyNet from "~/components/SlideNumpyNet";

export default {
  components: {
    SlideKerasNet, SlideTensorFlowNet,SlideNumSharp,SlideNumpyNet,
  },
  head () {
    return {
      title: "SciSharp STACK",
      meta: [
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { hid: 'description', name: 'description', content: 'A .NET based Open Source Ecosystem for Data Science, Machine Learning and AI' }
      ]
    }
  }
}
</script>
