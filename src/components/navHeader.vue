<template>
    
    <v-app-bar    
        color="grey-lighten-2"> 
      <v-btn color="red" icon="mdi-magnify"></v-btn>
            <template v-slot:prepend>
            <router-link to="/">

            
            <v-img
            :width="200"
            aspect-ratio="16/19"
            cover
            class=" mx-auto"
            src="https://unc.edu.ph/wp-content/uploads/2022/04/UNC-Logo-New.webp" 
            ></v-img>
        </router-link>
            </template>
      </v-app-bar>
      <v-app-bar
        color="red">
  <v-container class=" auto">
    <v-row d-flex justify="center">
      
      <v-col cols="auto">
        <v-btn density="default" to="/Humss" class=" mx-7">HUMSS</v-btn>
      </v-col>

      <v-col cols="auto">
        <v-btn density="default" to="/GAS" class=" mx-7">GAS</v-btn>
      </v-col>

      <v-col cols="auto">
        <v-btn density="default" to="/abm" class="mx-7">ABM</v-btn>
      </v-col>

      <v-col cols="auto">
        <v-btn density="default" to="/stem" class=" mx-7">STEM</v-btn>
      </v-col>

      <v-col cols="auto">
        <v-btn density="default" to="/tvl" class=" mx-7">TVL</v-btn>
      </v-col>
      
      <v-col cols="auto">
        <v-btn density="default" to="/ict" class=" mx-7">ICT</v-btn>
      </v-col>

      <v-col cols="auto">
        <v-btn density="default" to="/HE" class=" mx-7">HE</v-btn>
      </v-col>

    </v-row>
  </v-container>
  </v-app-bar>

</template>