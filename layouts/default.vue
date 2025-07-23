<template>
  <v-layout ref="app" class="flex-column rounded rounded-md border">
    <GlobalNav />

      <v-card>
        <v-layout>
          <v-navigation-drawer
            class="mt-6"
            expand-on-hover
            rail
          >

            <v-list class="global-nav" density="compact" nav>
              <NuxtLink to="/"><v-list-item prepend-icon="mdi-home" title="Home" value="home"></v-list-item></NuxtLink>
              <NuxtLink to="/type"><v-list-item prepend-icon="mdi-text-shadow" title="Text" value="text"></v-list-item></NuxtLink>

            </v-list>
          </v-navigation-drawer>

          <v-main class="d-flex align-center justify-center"  >
            <slot />
          </v-main>
        </v-layout>
      </v-card>
    <GlobalFooter />

  </v-layout>
</template>
<script setup>
  import { ref } from 'vue'

  const app = ref()

  function print (key) {
    alert(JSON.stringify(app.value.getLayoutItem(key), null, 2))
  }
</script>