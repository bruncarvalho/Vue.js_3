<template>
    <div>
      <button v-on:click.self="onClick">
        Enviar
      </button>
      <br>

      <div 
          @mouseover="onMouseOver"
          @mouseout="onMouseOut"
      
      >
        Mouse over
      </div>

      <br><br>

      <form 
        action="https://google.com"
        @submit.prevent="onSubmit"
      >

        <input 
        type="text"
        @keyup.delete="onKeyUp"
        >

        <button type="submit">
           Enviar 
        </button>
      
      </form>

    </div>     
</template>
    
    <script>
      export default {
      name: 'App',
      data(){
        return {
    
        }
      },
          methods: {
            onClick(event){
              console.log('click', event);
            },
            onMouseOver(event){
              console.log('mouse over', event);
            },
            onMouseOut(event){
              console.log('mouse out', event);
            },
            onSubmit(event){
              console.log('submit', event);
            },
            onKeyUp(event){
              console.log('onKeyUp', event);
            },
        }
      }
    </script>