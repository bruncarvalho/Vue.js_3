<template>
<div>
  <TheHeader v-if="showHeader"/>
  <h1>
    Hello World
  </h1>
  {{name}} <br>
  <input 
  v-model="name"
  type="text">
  <button @click="showHeader = !showHeader">
    Habilitar e desabilitar Header
  </button>
</div>
</template>

<script>
import TheHeader from './TheHeader.vue';
  export default {
    name: "App",
    data() {
        return {
            name: "Bruna Carvalho",
            showHeader: false
        };
    },
    // Criação
    //     Preparar o compontente
    //     Ajax, iniciar algumas variáveis
    //     Não tem acesso ao template (DOM)
    // Montagem
    //   Inicializar uma lib externa
    //   Geralmente precisa de acesso ao template
    //   Tem acesso ao template (DOM)
    // Atualização
    //   Debug
    //   Update
    // Desmontagem
    //   Remover tudo o que for necesário para liberar memória


    //HOOKS
    // beforeUpdate(){
    //   console.log('beforeUpdate')
    // },
    // updated(){
    //   console.log('updated')
    // },
    // beforeCreate() {
    //     console.log("Antes do componete ser criado");
    //     console.log("Estado:", this.name);
    //     console.log("DOM:", this.$el);
    // },
    // created() {
    //     console.log("criado");
    //     console.log("Estado:", this.name);
    //     console.log("DOM:", this.$el);
    // },
    // beforeMount() {
    //     console.log("Antes do componete ser montado");
    //     console.log("Estado:", this.name);
    //     console.log("DOM:", this.$el);
    // },
    // mounted() {
    //     console.log("Montado");
    //     console.log("Estado:", this.name);
    //     console.log("DOM:", this.$el);
    // },
    // beforeUnmount() {
    //     console.log("Antes do componete ser desmontado");
    //     console.log("DOM:", this.$el);
    // },
    // unmounted() {
    //     console.log("Desmontado");
    //     console.log("DOM:", this.$el);
    // },
    watch: {},
    computed: {},
    methods: {},
    components: { TheHeader }
}


</script>