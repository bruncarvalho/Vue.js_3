<template>
  
  <div id="app">
    <TheHeader
    
    />

    <vBind
    
    />
  </div>

</template>

<script>

import TheHeader from './components/TheHeader.vue';
import vBind from './components/vBind.vue'

export default {
  name: 'App',
  components: {
      TheHeader,
      vBind
  }
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  color: #2c3e50;
  margin: 60px;
}
</style>
