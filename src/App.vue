<template>
  
  <div id="app">
    <TheHeader/>

    <vBind/>

    <vModel/>

    <Events/>

  </div>

</template>

<script>

// import TheHeader from './components/TheHeader.vue';
// import vBind from './components/vBind.vue';
// import vModel from './components/vModel.vue';
import Events from './components/Events.vue'

export default {
  name: 'App',
  components: {
      // TheHeader,
      // vBind,
      // vModel,
      Events
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
