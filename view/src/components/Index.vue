<template>
  <v-app>
    <Header/>
    <br>
    <v-container fill-height>
    <v-row align="center"
      justify="center" >
        <v-col align="left">
            <v-img
                src="../assets/doctor-blue.png"
                contain="true"
                max-height="780"
                position="center"
            ></v-img>
        </v-col>
        <v-col align="center">
           <h1 style="color:#00BFA6">Welcome to your new planner</h1>
           <br>
           <v-btn
            color="#00BFA6"
            elevation="24"
            large
            x-large
            href="/login"
            >Log In</v-btn>
        </v-col>
    </v-row>
</v-container>
<br>
    <Footer/>
  </v-app>
</template>

<script>
import Header from '@/components/Header';
import Footer from '@/components/Footer';

export default {
  name: 'Index',

  components: {
    //HelloWorld,
    Header,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>