<template>
  <div id="app">
    <circles />
    <card />
  </div>
</template>

<script>
import card from './components/card'
import circles from './components/circles'

export default {
  name: 'App',
  components: {
    card,
    circles
  }
}
</script>

<style lang="scss">
body {
  overflow: hidden;
}
#app {
  background: linear-gradient(to left, #283593, #1976d2);
  width: 100vw;
  height: 100vh;
}
</style>
