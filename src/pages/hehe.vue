<template>
    <div>
      <div class="red-bar text-white mt-16" style="background-color: red; padding: 10px 20px;">
        <h1 class="text-center m-0">
        SHS EVENTS
        </h1>
      </div>
      
      <div class="text-center mt-6">
        <h2 class="text-h5 font-weight-black text-red mt-10 mb-10">
          {{ programOutcomes[currentIndex] }}
        </h2>
      </div>
  
      <v-carousel class="mt-6" v-model="currentIndex">
        <v-carousel-item v-for="(item, index) in carouselItems" :key="index">
          <img :src="item.src" :alt="'Image ' + (index + 1)">
          <div class="text-h6 mt-2">{{ item.text }}</div>
        </v-carousel-item>
      </v-carousel>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        currentIndex: 0,
        programOutcomes: [
          "INTRAMURALS",
         "A SPECIAL EVENT FOR EACH STRANDS",
           "CAREER FAIR",
          "STRAND-SPECIFIC ALUMNI PANEL",
          "CAREER EXPLORATION FAIR"
        ],
        carouselItems: [
          { src: "image1.jpg", text: "The UNC intramurals is an exciting and inclusive part of our school's extracurricular program! These are organized sports and recreational activities that take place right here on our campus. It's all about students coming together to participate in friendly competitions and fun games within our school community. Whether you're into basketball, soccer, volleyball, or other recreational activities, there's something for everyone to enjoy." },
          { src: "image2.jpg", text: "Get ready to be surprised at our Program Outcome event crafted for each strand with you in mind! Dive into humanities, business, arts, or technical skills and join us for a day of fun, connection, and unexpected delights, no matter your focus." },
          { src: "image3.jpg", text: "Where students can explore various career options, meet professionals from different industries, and learn about educational pathways and job opportunities." },
          { src: "image4.jpg", text: "This event brings together alumni who graduated from the same senior high school strand to share their post-graduation experiences, career paths, and insights with current students. It provides an opportunity for students to learn firsthand about the benefits and opportunities associated with pursuing a particular strand and how it can lead to various career pathways and successes in college and beyond." },
          { src: "image5.jpg", text: "Organize a fair where students can explore various career options through interactive exhibits, informational booths, and guest speakers representing different industries and professions. This event helps students gain insights into potential career paths and make informed decisions about their future." }
        ]
      };
    }
  };
  </script>