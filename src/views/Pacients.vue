<template>
<div>
  <v-row no-gutters>
    <v-col cols="1">
      <Navbar/>
    </v-col>
    <v-col cols="11">
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
