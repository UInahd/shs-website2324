<template>   
  <v-app theme="light" class="cover-bg " >
      <navHeader/>

      <v-container class="mt-16">
        <v-row class="py-16 my-16">
          <v-col>
            <h3 class="text-h2 font-weight-bold mt-16 mx-6"> Humanities and Social Science Strand  </h3>
            
            <v-btn
            width="120"
            height="40"
            color="red"
            justify="auto"
            class="text-white font-weight-bold center mt-6 mx-6 auto">Apply Now!
          </v-btn>
          </v-col>

          <v-col>
            <div style="position: absolute; top: 250px; right: 20px; text-align: auto; opacity: 0.3; " >
            <img draggable="false" src="@/assets/HUMMSlogo.png" style="width:auto;height:900px;">
          </div>
          </v-col>

        </v-row>
      <v-row>
        <v-col>
          <v-img class="mt-16 pe-16" src="../assets/pic1.png"> </v-img>
          
        </v-col>
        <v-col>
          <div class="text-justify ">
            <h2 class="text-h4 font-weight-normal mt-16 mx-8 "> 
              <strong class="text-red">Human and Social Science</strong> </h2>
                <h2 class="text-h5 font-weight-normal mt-6 mx-8 ">
                  The <b>Humanities and Social Sciences (HUMMS)</b>
                  strand in senior high school
                  is designed to effectively prepare
                  students who seek to pursue a college
                  degree in liberal education. HUMSS courses
                  cover a variety of subjects, looking at the
                  world and its people from various points of
                  view. The learning activities are directed
                  towards the development of critical thinking.
                </h2>
          </div>

        </v-col>
        
      </v-row>
      <v-row>
        <v-col>
          <div class="text-justify ">
            <h2 class="text-h5 font-weight-normal mt-6 mx-8 ">
              The <b>Humanities and Social Sciences (HUMMS)</b> 
              strand is an educational track designed
              to provide students with a comprehensive understanding
              of various disciplines such as history, literature,
              sociology, psychology, and economics. It focuses on
              developing critical thinking skills, cultural awareness,
              and effective communication abilities through a diverse
              range of subjects.
            </h2>
          </div>
          
          
        </v-col>
        <v-col>
          
            <v-img class="mt-16 pe-16" src="../assets/pic2.png" > </v-img>
            
           
        </v-col>
      </v-row>
    </v-container>
        <div class="text-red mt-16">
        <text class="text-h4 ">
          <h1 class="text-center ">
            
              Program Outcome
          </h1>
        </text>
              </div>
             
              <text class="text-center">
                <h2 class="text-h5 font-weight-normal mt-10 mb-10">
                  By the end of school year, the HUMMS learners shall have the ability to:
                </h2>
              </text>
            </v-app>
              <v-carousel height="800">

                <v-carousel-item src="@/assets/image1.jpg" cover>
                  <div class="  bg-black bottom-0 overlay" >
                    <p class="title font-weight-bold text-h3 text-left ma-16 pa-16 text-white w-100">
                    1. Acquire the appropriate mindset and theorems for understanding the psyche and behavior of people across different backgrounds.
                  </p>     
                  </div>
                        
                      </v-carousel-item>
                      <v-carousel-item src="@/assets/image2.jpg" cover>
                        <div class="  bg-black bottom-0 overlay" >
                          <p class="title font-weight-bold text-h3 text-left ma-16 pa-16 text-white w-100">
                          2. Build their confidence in articulating their various ideas and expressing themselves through both written and spoken language in both scholarly and secular work.
                        </p>
                        </div>
                        
                      </v-carousel-item>
                      <v-carousel-item src="@/assets/image3.png" cover>
                        <div class="bg-black bottom-0 overlay" >
                          <p class="title font-weight-bold text-h3 text-left ma-16 pa-16 text-white w-100">
                          3. Provide them with the means to gaining the necessary rapport with their future patients, clients, audiences, and other stakeholders depending on their profession of choice.
                        </p>
                        </div>
                        
                      </v-carousel-item>
                    </v-carousel>
                  
            

                <v-card>
                  <v-tabs
                    v-model="tab"
                    bg-color="red" fixed-tabs
                  >
                    <v-tab value="one">EVENT</v-tab>
                    <v-tab value="two">SUBJECT</v-tab>
                    <v-tab value="three">FEEDBACK</v-tab>
                  </v-tabs>
              
                  <v-card-text>
                    <v-tabs-window v-model="tab">
                      <v-tabs-window-item value="one">
                      <Event></Event>
                      </v-tabs-window-item>
              
                      <v-tabs-window-item value="two">
                       <subject></subject>
                      </v-tabs-window-item>
              
                      <v-tabs-window-item value="three">
                        <feedback></feedback>
                      </v-tabs-window-item>
                    </v-tabs-window>
                  </v-card-text>
                </v-card>        
    
<Hfooter></Hfooter>

</template>


<script setup>
import navHeader from '../components/navHeader.vue';
import Hfooter from '../components/footer.vue';
</script>
<script>
import Event from "../components/hummEvent.vue"
import feedback from "../components/abmfeedback.vue"
import subject from "../components/hummsSubject.vue"


export default {
  
  components: {
    Event,
    feedback,
    subject
  },
  data () { 
    return {
      tab: null,
      event: true,
      subject: false,
      feedback: false,
      isCollapsed: true
    };
  },
  methods: {
    toggleCollapse() {
      this.isCollapsed = !this.isCollapsed;
    }
  }
};
</script>

<style>

  .title {
    margin-left: 0%;
    text-align: center;
    position: absolute;
    bottom: 50px;
    background-color: rgba(0,0,0,0.5);
    color: white;
    font-size: 1em;
    padding: 20px;
  }
  .img draggable{
    background-size: cover;
  }
  .cover-bg{
    background-image: url('@/assets/weball.png'); 
  }
</style>