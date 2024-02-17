<template>
  <div>
    <Greet />
  </div>
</template>

<script>
import Greet from './components/GreetPpl.vue'

export default {
  name: 'App',
  components: {
    Greet,
  }
}
</script>

<style scoped>
#app {
  font-family: 'Times New Roman', Times, serif;
}
</style>