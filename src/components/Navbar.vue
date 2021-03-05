<template>
  <nav>
    <v-navigation-drawer  v-model="drawer" dark mini-variant mini-variant-width="150" color="#00BFA6" class="darken-1">
        <v-list>
              <v-list-item class="mb-12">
                <v-list-item-action>
                </v-list-item-action>
            </v-list-item >
        </v-list>
        <v-list flat>
          <v-list-item  router to="/dashboard">
            <v-list-item-content>
                <v-icon class="mb-2">dashboard</v-icon>
                <v-list-item-subtitle align="center">Dasboard</v-list-item-subtitle>
            </v-list-item-content>  
        </v-list-item>
        </v-list>
        <v-list>
              <v-list-item class="mb-12">
                <v-list-item-action>
                </v-list-item-action>
            </v-list-item >
        </v-list>
        <v-list flat>
        <v-list-item  router to="/pacients">
              <v-list-item-content>
                <v-icon class="mb-2">fas fa-user-injured</v-icon>
                <v-list-item-subtitle align="center">Pacient</v-list-item-subtitle>
            </v-list-item-content>  
        </v-list-item>
        </v-list>
        <v-list>
              <v-list-item class="mb-14">
                <v-list-item-action>
                </v-list-item-action>
            </v-list-item >
        </v-list>
        <v-list flat>
        <v-list-item  router to="/appointments">
              <v-list-item-content>
                <v-icon class="mb-2">far fa-calendar-check</v-icon>
                <v-list-item-subtitle align="center">Appointment</v-list-item-subtitle>
            </v-list-item-content>  
        </v-list-item>
        </v-list>
        <v-list>
              <v-list-item class="mb-16">
                <v-list-item-action>
                </v-list-item-action>
            </v-list-item >
        </v-list>
        <v-list>
              <v-list-item class="mb-14">
                <v-list-item-action>
                </v-list-item-action>
            </v-list-item >
        </v-list>
        <v-list  style="position: absolute; bottom:0" class="ml-10" flat>
          <v-list-item  router to="/signout">
                <v-list-item-action>
                    <v-icon right>fas fa-sign-out-alt</v-icon>
                </v-list-item-action>
            </v-list-item>
        </v-list>
    </v-navigation-drawer>
  </nav>
</template>