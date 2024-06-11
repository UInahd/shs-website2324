<template>
<v-sheet :elevation="22" :height="200" :width="200" style="width: 35%; height: 50%; position: absolute; left:32%; bottom: 200px;">

    <v-container :width="200">
<h1 class="text-left">We’d love to hear from you!</h1>
<p class="text-left">Rate your experience.</p>

  <div class="text-center">
    <v-rating
      v-model="rating"
      active-color="red"
      color="gray"
    ></v-rating>
  </div>
  <p>Tell us what can be Improved?</p>
  <v-textarea label="Write your suggestion here..."></v-textarea>
  <p>Read feedbacks from students.</p>
  <v-btn color="red" style="position: fixed; font-size: 15px; right:35%;" size="large" class="right-0" >
    Submit
  </v-btn>
  </v-container>

</v-sheet>
</template>
<script>

</script>

<style>

</style>