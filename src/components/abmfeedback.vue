<template>
    <v-card
      class=" mt-16 mx-auto"
      
      subtitle="Rate your experience."
      width="400"
      height="450"
    >

      <template v-slot:title>
        <span class="font-weight-black">We’d love to hear from you!</span>
      </template>
  
      <div class="text-center">
    <v-rating
      v-model="rating"
      active-color="red"
      color="black"
      size="x-large"
    ></v-rating>
  </div>
<h3 class= "text-left ml-6">Tell us what can be Improved?</h3>
  <v-app>
    <v-container class="text-right" >
      <v-textarea label="Write your suggestion here..."></v-textarea>
      <v-btn 
      color="red"
      variant="flat"
      >Submit
</v-btn>

    </v-container>
  </v-app>
        </v-card>


        <h1 class="text-center text-red mt-10 font-weight-bold"
        
              > What do students say?</h1>

              <h3 class="text-center mt-1 mb-10 font-weight-normal"
        
              > Hear from current and former students about their experiences in this particular strand.</h3>


      <v-app>
    <v-container >
      <v-carousel class="mx-auto" elevation="24"  height="500">
       
        <v-carousel-item class="text-center"  ><v-avatar  size="100">
      <v-img  alt="John" src="https://i.pinimg.com/736x/c2/81/fd/c281fdbeeff1de5076707463c48304d3.jpg"></v-img>
    </v-avatar>
          <v-card-title class="text-center text-h4"> Jobert Tuazon </v-card-title>
          Current Student
          <v-card class="mx-auto mt-10" height="170" max-width="444" hover>


    <v-card-text class="ma-4">
      "My experience there has been nothing short of amazing. The teachers are extremely dedicated and passionate 
      about what they do, and they always go the extra mile to help us succeed. 
      The curriculum is top-notch and really challenges us to think critically and problem-solve"
    </v-card-text>
  </v-card>
          </v-carousel-item
        >

        <v-carousel-item class="text-center"  ><v-avatar  size="100">
      <v-img  alt="John" src="https://cdn.vuetifyjs.com/images/john.jpg"></v-img>
    </v-avatar>
          <v-card-title class="text-center text-h4"> Kobie James </v-card-title>
          Current Student
          <v-card class="mx-auto mt-10" height="170" max-width="444" hover>


    <v-card-text class="ma-5">
      "The school offers a wide range of extracurricular activities, which has allowed me to explore 
      my interests and develop new skills. Overall, I couldn't be happier with my choice to attend this school. 
      It has truly been a transformative experience for me.."
    </v-card-text>
  </v-card>
          </v-carousel-item
        >

        <v-carousel-item class="text-center"  ><v-avatar  size="100">
      <v-img  alt="John" src="https://i.pinimg.com/564x/14/03/3b/14033bc98b6a00eed4483fa951bf0e79.jpg"></v-img>
    </v-avatar>
          <v-card-title class="text-center text-h4"> Francis De Leon </v-card-title>
          Current Student
          <v-card class="mx-auto mt-10" height="200" max-width="444" hover>


    <v-card-text class="ma-3">
      "I absolutely love my school! The community is so supportive and the teachers are 
      amazing. They really care about each student's success and go above and beyond to help us learn and grow.
       The resources available to us are top-notch and I always feel challenged 
      in a positive way. Overall, I couldn't be happier with my experience at this school."
    </v-card-text>
  </v-card>
          </v-carousel-item
        >
      </v-carousel>
    </v-container>
  </v-app>


  </template>
  <script>
  export default {
    data: () => ({ rating: 3 }),
  }
</script>