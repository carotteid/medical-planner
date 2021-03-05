<template>
    <v-container fill-height>
        <v-row align="center"
          justify="center" no-gutters >
            <v-col align="left" cols="7">
                <v-img
                    src="../assets/doctor-blue.png"
                    contain="true"
                    max-height="700"
                    position="center"
                ></v-img>
            </v-col>
            <v-col align="center" cols="5">
              <h1 style="color:#00BFA6; font-size:40px">Welcome to your new planner</h1>
              <br>
              <v-btn
                color="#00BFA6"
                elevation="6"
                large
                x-large
                href="/login"
                >Log In</v-btn>
                <br>
                <br>
                <p>If you don't have an account, <a href="/signup">Sign Up</a>.</p>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
  }
}
</script>
