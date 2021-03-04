<template>
  <v-card class="overflow-hidden">
    <v-app-bar
      absolute
      color="#00BFA6"
      elevate-on-scroll
    >
      
      <v-toolbar-title>Medical Planner</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-app-bar-nav-icon></v-app-bar-nav-icon>
    </v-app-bar>
    <v-sheet
      id="scrolling-techniques-7"
      class="overflow-y-auto"
    >
      <v-container style="height: 805px;"> </v-container>
    </v-sheet>
  </v-card>
</template>
<template>
  <div>
    <v-app-bar
      color="#00BFA6"
      dense
    >
    <v-img
        src="../assets/heart.png"
        contain="true"
        height="40"
        position="left"
        ></v-img>

      <v-menu
        left
        bottom
      >
        <template v-slot:activator="{ on, attrs }">
          <v-btn
            icon
            v-bind="attrs"
            v-on="on"
          >
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>

        <v-list>
          <v-list-item>
            <v-list-item-title>Log In</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title>Sign Up</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>

    </v-app-bar>
  </div>
</template>
