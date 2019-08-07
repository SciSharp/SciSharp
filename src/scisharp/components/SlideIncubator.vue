<template>
    <div class="slide pa-5 bg1" id="incubator">
        <v-layout column
                  text-xs-center
                  wrap
                  class="pb-5"
        >
            <v-flex xs12>
                <img
                        src="@/assets/incubator.svg"
                        class="mt-5 mb-0"
                        height="300"
                        alt="Incubator"
                ></img>
            </v-flex>

            <v-flex mb-5>
                <h2 class="display-1 font-weight-light mb-3 white--text">
                    What else is in the making?
                </h2>
                <p class="title font-weight-light mb-3 white--text">
                    Projects that are Alpha or Work-in-progress
                </p>
            </v-flex>

            <v-flex>
                <v-layout row wrap mx-5>
                    <v-spacer></v-spacer>
                    <v-flex xs4 mx-5>
                        <v-list two-line class="bg1">

                            <v-list-item href="https://github.com/SciSharp/Torch.NET" target="_blank" @click="">
                                <v-list-item-avatar>
                                    <img src="@/assets/Torch.NET_icon_transparent.svg" width="48" height="48" alt="Torch.NET"></img>
                                </v-list-item-avatar>
                                <v-list-item-content>
                                    <v-list-item-title>Torch.NET</v-list-item-title>
                                    <v-list-item-subtitle>.NET bindings for PyTorch. Machine Learning with C# / F# with Multi-GPU/CPU support</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>

                            <v-list-item href="https://github.com/SciSharp/Gym.NET" target="_blank" @click="">
                                <v-list-item-avatar>
                                    <v-icon>fab fa-github</v-icon>
                                </v-list-item-avatar>
                                <v-list-item-content>
                                    <v-list-item-title>Gym.NET</v-list-item-title>
                                    <v-list-item-subtitle>A pure C# implementation of OpenAI/Gym Reinforcement Learning Environments</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>

                            <v-list-item href="https://github.com/SciSharp/Pandas.NET" target="_blank" @click="">
                                <v-list-item-avatar>
                                    <v-icon>fab fa-github</v-icon>
                                </v-list-item-avatar>
                                <v-list-item-content>
                                    <v-list-item-title>Pandas.NET</v-list-item-title>
                                    <v-list-item-subtitle>A pure C# port of the Pandas Data Analysis Library</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>

                            <v-list-item href="https://github.com/SciSharp/Matplotlib.Net" target="_blank" @click="">
                                <v-list-item-avatar>
                                    <v-icon>fab fa-github</v-icon>
                                </v-list-item-avatar>
                                <v-list-item-content>
                                    <v-list-item-title>Matplotlib.Net</v-list-item-title>
                                    <v-list-item-subtitle>.NET wrapper for the Python plotting library Matplotlib</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>

                            <v-list-item href="https://github.com/SciSharp/CherubNLP" target="_blank" @click="">
                                <v-list-item-avatar>
                                    <v-icon>fab fa-github</v-icon>
                                </v-list-item-avatar>
                                <v-list-item-content>
                                    <v-list-item-title>CherubNLP</v-list-item-title>
                                    <v-list-item-subtitle>Natural Language Processing in .NET Core</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>

                            <v-list-item href="https://github.com/SciSharp/scikit-learn.net" target="_blank" @click="">
                                <v-list-item-avatar>
                                    <v-icon>fab fa-github</v-icon>
                                </v-list-item-avatar>
                                <v-list-item-content>
                                    <v-list-item-title>scikit-learn.net</v-list-item-title>
                                    <v-list-item-subtitle>A pure C# implementation of SciKit Learn</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>

                        </v-list>
                    </v-flex>

                    <v-flex xs4 mx-5>
                        <v-list two-line class="bg1">

                            <v-list-item href="https://github.com/SciSharp/BotSharp" target="_blank" @click="">
                                <v-list-item-avatar>
                                    <v-icon>fab fa-github</v-icon>
                                </v-list-item-avatar>
                                <v-list-item-content>
                                    <v-list-item-title>BotSharp</v-list-item-title>
                                    <v-list-item-subtitle>A pure C# AI Chatbot Platform Builder</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>

                            <v-list-item href="https://github.com/SciSharp/OpenAIGym.NET" target="_blank" @click="">
                                <v-list-item-avatar>
                                    <v-icon>fab fa-github</v-icon>
                                </v-list-item-avatar>
                                <v-list-item-content>
                                    <v-list-item-title>OpenAIGym.NET</v-list-item-title>
                                    <v-list-item-subtitle>A toolkit for developing and comparing reinforcement learning algorithms</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>

                            <v-list-item href="https://github.com/SciSharp/mxnetlib" target="_blank" @click="">
                                <v-list-item-avatar>
                                    <v-icon>fab fa-github</v-icon>
                                </v-list-item-avatar>
                                <v-list-item-content>
                                    <v-list-item-title>MxNetLib</v-list-item-title>
                                    <v-list-item-subtitle>.NET Bindings for Apache MXNET, a Scalable Deep Learning Framework</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>

                            <v-list-item href="https://github.com/SciSharp/Ludwig.NET" target="_blank" @click="">
                                <v-list-item-avatar>
                                    <v-icon>fab fa-github</v-icon>
                                </v-list-item-avatar>
                                <v-list-item-content>
                                    <v-list-item-title>Ludwig.NET</v-list-item-title>
                                    <v-list-item-subtitle>.NET Bindings for Ludwig. Train and test deep learning models without writing code.</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>

                            <v-list-item href="https://github.com/SciSharp/Microcharts.Matplotlib" target="_blank" @click="">
                                <v-list-item-avatar>
                                    <v-icon>fab fa-github</v-icon>
                                </v-list-item-avatar>
                                <v-list-item-content>
                                    <v-list-item-title>Microcharts.Matplotlib</v-list-item-title>
                                    <v-list-item-subtitle>.NET wrapper of Microcharts for Data Science and Machine Learning</v-list-item-subtitle>
                                </v-list-item-content>
                            </v-list-item>

                        </v-list>
                    </v-flex>

                    <v-spacer></v-spacer>
                </v-layout>
<!--                <v-btn-->
<!--                        text large outlined-->
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
        </v-layout>

    </div>

</template>

<script>
    export default {
        name: "SlideTensorFlowNet"
    }
</script>

<style scoped>

</style>