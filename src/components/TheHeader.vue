<template>
  <header class="header">
    Header
  </header>
</template>

<script>
  export default {
    mounted() {
      window.addEventListener('resize', this.resize)
    },

    beforeUnmount() {
        console.log("Antes do componete ser desmontado");
        console.log("DOM:", this.$el);
    },
    unmounted() {
        console.log("Desmontado");
        console.log("DOM:", this.$el);
    },

    methods: {
      resize($evt) {
        console.log($evt);
      }
    }
  }
  
 
</script>

<style>
  .header {
      background: #000;
      color: #fff;
  }
</style>