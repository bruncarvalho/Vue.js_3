<template>
<div>
  <h1>
    Hello World
  </h1>
  {{name}}
</div>
</template>

<script>
  export default {
    name: 'App',
    data() {
      return{
        name: 'Bruna Carvalho'
      }
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
      beforeCreate() {
        console.log('Antes do componete ser criado');
        console.log('Estado:', this.name);
        console.log('DOM:', this.$el);
      },
      created() {
        console.log('criado');
        console.log('Estado:', this.name);
        console.log('DOM:', this.$el);
      },
      beforeMount() {
        console.log('Antes do componete ser montado');
        console.log('Estado:', this.name);
        console.log('DOM:', this.$el);
      },
      mounted(){
        console.log('Montado')
        console.log('Estado:', this.name);
        console.log('DOM:', this.$el);
      },
      beforeUnmount() {
        console.log('Antes do componete ser desmontado');
        console.log('DOM:', this.$el);
      },
      unmounted(){
        console.log('Desmontado');
        console.log('DOM:', this.$el);
      },


    watch: {

    },
    computed: {

    },
    methods: {

    }
  }


</script>