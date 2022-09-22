<template>
  
  <div id="app">
    <!-- <vif_vfor/> -->

    <TheHeader/>

   <!--  <vBind/>

    <vModel/>

    <Events/>

    <computed/>

    <watch/> -->

    <lifeCycle/>


  </div>

</template>

<script>

import TheHeader from './components/TheHeader.vue';
// import vif_vfor from './components/vif_vfor.vue';
// import vBind from './components/vBind.vue';
// import vModel from './components/vModel.vue';
// import Events from './components/Events.vue';
// import computed from './components/computed.vue';
// import watch from './components/watch.vue';
import lifeCycle from './components/lifeCycle.vue'

export default {
  name: 'App',
  components: {
      TheHeader,
      // vif_vfor,
      // vBind,
      // vModel,
      // Events,
      // computed,
      // watch,
      lifeCycle
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
