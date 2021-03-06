<template>
<div>
  <v-row no-gutters>
    <v-col cols="1">
      <Navbar/>
    </v-col>
    <v-col cols="11">
        <br>
        <v-content align="right">
        <v-btn
        color="#00BFA6"
        elevation="2"
        fab
        x-large
        align="right"
        dark
        href="/appointments/add"
      >
      <v-icon>fas fa-plus</v-icon>
      </v-btn>
      </v-content>
      <br>
      <v-content>
        <v-data-table
            :headers="headers"
            :items="desserts"
            class="elevation-1"
        ></v-data-table>
      </v-content>
    </v-col>
  </v-row>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar';

export default {
  name: 'App',

  components: {
    //HelloWorld,
    Navbar
  },

  //TODO: conect database 
  data: () => ({
    })
};
</script>
