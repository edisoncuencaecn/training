<template>
<v-app-bar class="global-nav" density="compact" :elevation="2" theme="dark">
  <template v-slot:prepend>
    <v-app-bar-nav-icon class="pl-3">
      <img src="../assets/img/gc-logos/img_forest.jpg" alt="" width="44" height="22" />
    </v-app-bar-nav-icon>
  </template>
  <v-app-bar-title>Forces.ca Style Guide</v-app-bar-title>
    <div>
        <ul>
          <li>1</li>
          <li>2</li>
          <li>3</li>
          <li>4</li>
        </ul>
      </div>
  <template v-slot:append>
      <v-btn prepend-icon="mdi-home"><NuxtLink to="/">Home</NuxtLink></v-btn>
      <v-btn prepend-icon="mdi-text-shadow"><NuxtLink to="/type">Type</NuxtLink></v-btn>
      <v-btn icon="mdi-magnify"></v-btn>
    <v-btn icon="mdi-dots-vertical"></v-btn>
  </template>
</v-app-bar>
</template>
