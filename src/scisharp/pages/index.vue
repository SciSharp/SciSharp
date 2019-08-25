<template>
    <v-layout column id="hmm">

        <!--    main screen-->
        <v-container class="slide mt-0 pa-0" fluid>
            <v-layout column
                      text-center
                      wrap
            >
                <v-flex xs12 style="min-height: 250px;">
                    <v-img
                            :src="require('@/assets/scisharp-stack.svg')"
                            contain
                            class="mt-5 mb-2"
                            height="250"
                            max-height="250"
                            alt="SciSharp STACK"
                    ></v-img>
                </v-flex>

                <v-flex xs12 mb-5>
                    <h2 class="display-1 font-weight-light mb-3 white--text">
                        A .NET based Open Source Ecosystem for Data Science, Machine Learning and AI
                    </h2>
                    <p class="title font-weight-light mb-5 white--text">
                        SciSharp brings all major ML/AI Frameworks from Python to .NET
                    </p>
                </v-flex>
            </v-layout>
            <div class="bg2">
                <v-container style="max-width: 1600px;">
                    <v-layout row wrap justify-center fill-height my-5 mx-5 >
                        <v-flex xs12 sm6 lg3 px-2 py-2>
                            <v-card light :style="dynamic_card_style" elevation-5>
                                    <v-card-title>
                                        For .NET Developers
                                    </v-card-title>
                                    <v-card-text class="text-left">
                                        .NET developers are most productive with the <b>tools they know and love</b>. Our
                                        mission is to make sure
                                        that they don't have to leave that behind when reaching for opportunities in Data
                                        Science Machine Learning and AI.
                                        The well established Python
                                        based Machine Learning ecosystem is not quite accessible to millions of .NET developers.
                                        We are effectively
                                        changing that.
                                    </v-card-text>
                            </v-card>
                        </v-flex>

                        <v-flex  xs12 sm6 lg3 px-2 py-2>
                            <v-card light :style="dynamic_card_style" elevation-5>
                                <v-card-title>
                                    Cutting Edge
                                </v-card-title>
                                <v-card-text class="text-left">
                                    SciSharp provides ports and bindings to cutting edge Machine Learning frameworks like
                                    <b>TensorFlow</b>,
                                    <b>Keras</b>, <b>PyTorch</b>, <b>Numpy</b> and many more in .NET Core. Since the APIs of
                                    the ported libraries are so similar
                                    to the originals you can easily re-use all existing resources, documentation and
                                    community solutions to
                                    common problems in C# or F# without much effort.
                                </v-card-text>
                            </v-card>
                        </v-flex>

                        <v-flex  xs12 sm6 lg3 px-2 py-2>
                            <v-card light :style="dynamic_card_style" elevation-5>
                                <v-card-title>
                                    Cross-Platform
                                </v-card-title>
                                <v-card-text class="text-left">
                                    All libraries of the SciSharp STACK target the cross-platform <b>.NET Standard
                                    Framework</b>, which makes them
                                    usable on any major platform that supports .NET Core. We provide a ready-made Docker
                                    image with Jupyter Notebook
                                    being able to execute C# expressions and enabling you to start playing around with our
                                    libraries immediately.
                                </v-card-text>
                            </v-card>
                        </v-flex>

                        <v-flex  xs12 sm6 lg3 px-2 py-2>
                            <v-card light :style="dynamic_card_style" elevation-5>
                        <v-card-title>
                            Open Source
                        </v-card-title>
                        <v-card-text class="text-xs-left">
                            SciSharp libraries are licensed under permissive licences, such as the Apache 2.0
                            license, allowing you to use them for any purpose
                            including <b>commercial applications</b> as long as the copyright of the authors is
                            retained. The Open Source
                            nature of the SciSharp STACK is attracting many contributors who further extend and
                            improve it.
                        </v-card-text>
                    </v-card>
                        </v-flex>

                        <!--        </v-layout>-->
                        <!--      </v-flex>-->

                    </v-layout>
                </v-container>
            </div>
        </v-container>
        <SlideTensorFlowNet></SlideTensorFlowNet>
        <SlideNumSharp></SlideNumSharp>
        <SlideKerasNet></SlideKerasNet>
        <SlideNumpyNet></SlideNumpyNet>
        <SlideCatalystNlp></SlideCatalystNlp>
        <SlideNeuralNetworkNet></SlideNeuralNetworkNet>
        <SlideSciSharpCube></SlideSciSharpCube>
        <SlideCompanies/>
        <SlideIncubator></SlideIncubator>

        <Footer></Footer>
    </v-layout>

</template>


<script>
    import 'babel-polyfill'
    import SlideTensorFlowNet from '~/components/SlideTensorFlowNet.vue'
    import SlideNumSharp from '~/components/SlideNumSharp.vue'
    import SlideKerasNet from "~/components/SlideKerasNet";
    import SlideNumpyNet from "~/components/SlideNumpyNet";
    import SlideCatalystNlp from "../components/SlideCatalystNlp";
    import SlideSciSharpCube from "../components/SlideSciSharpCube";
    import SlideIncubator from "~/components/SlideIncubator";
    import SlideCompanies from "~/components/SlideCompanies";
    import SlideNeuralNetworkNet from "../components/SlideNeuralNetworkNet";
    import Footer from "../components/Footer";

    export default {
        components: {
            Footer,
            SlideNeuralNetworkNet,
            SlideSciSharpCube, SlideKerasNet, SlideTensorFlowNet, SlideNumSharp, SlideNumpyNet, SlideIncubator, SlideCatalystNlp, SlideCompanies
        },
        data: () => ({
        }),
        head() {
            return {
                title: "SciSharp STACK",
                meta: [
                    // hid is used as unique identifier. Do not use `vmid` for it as it will not work
                    {
                        hid: 'description',
                        name: 'description',
                        content: 'A .NET based Open Source Ecosystem for Data Science, Machine Learning and AI'
                    }
                ]
            }
        },
        computed: {
            dynamic_card_style () {
                if (this.$vuetify.breakpoint.xlOnly)
                    return { 'min-height':'250px' }
                if (this.$vuetify.breakpoint.lgOnly)
                    return { 'min-height':'300px' }
                if (this.$vuetify.breakpoint.mdOnly)
                    return { 'min-height':'220px' }
                if (this.$vuetify.breakpoint.smOnly)
                    return { 'min-height':'230px' }
                    if (this.$vuetify.breakpoint.smAndDown)
                return { }
            },
        },
    }
</script>
