<template>
  
  <div id="app">
    <TheHeader
      v-if="showHeader"
    />

    <div v-show="showName">
      Nome: {{ firstName }} <br>
      SobreNome: {{lastName}}
    </div>

    <div v-if="acessLevel === 'admin'">Usuário Admin</div>
    <div v-else-if="acessLevel === 'marketing'">Usuário Marketing</div>
    <div v-else>Usuário normal</div>
    
    <img 
    alt="Vue logo" src="./assets/logo.png"
    >
    <HelloWorld msg="Welcome to Your Vue.js App"/>
    
  </div>

</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import TheHeader from './components/TheHeader.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
      TheHeader
  },
  data() {
    return {
      showHeader: true,
      firstName: 'Bruna',
      lastName: 'Carvalho',
      showName: false,
      acessLevel: 'marketing'
    }
  }
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
