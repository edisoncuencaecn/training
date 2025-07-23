<template>
    <v-footer color="surface-light" name="footer">
      <h1>Footer</h1>
      <v-btn
        class="mx-auto"
        text="Get data"
        variant="text"
        @click="print('footer')"
      ></v-btn>
    </v-footer>
</template>

<script setup>
  import { ref } from 'vue'
  const app = ref()
  const key = ref(123)
  function print (key) {
    alert(JSON.stringify(app.value.getLayoutItem(key), null, 2))
  }
</script>
