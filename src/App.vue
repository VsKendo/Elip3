<template>
  <AppIndex />
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import AppIndex from './views/AppIndex.vue'

export default defineComponent({
  name: 'App',
  components: {
    AppIndex
  }
})
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
