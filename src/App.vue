<template>
  <NavBar/>
  <router-view/>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fee045;

}
html, body {
  background-color: #000000;
  overflow-x: hidden;
  overflow-y: auto;
}

</style>

<script >
export default {
  name: 'App'

}
</script>
