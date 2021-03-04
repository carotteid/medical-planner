<template>
  <v-card class="overflow-hidden">
    <v-app-bar
      absolute
      color="#00BFA6"
      elevate-on-scroll
      scroll-target="#scrolling-techniques-7"
    >
      <v-img
        src="../assets/heart.png"
        contain="true"
        height="50"
        position="left"
        ></v-img>
      <v-toolbar-title>Medical Planner</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-app-bar-nav-icon></v-app-bar-nav-icon>
    </v-app-bar>
    <v-sheet
      id="scrolling-techniques-7"
      class="overflow-y-auto"
      max-height="600"
    >
      <v-container style="height: 1500px;"> </v-container>
    </v-sheet>
  </v-card>
</template>
