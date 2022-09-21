<template>
 <div>
    <div>
      One-way data binding <br/>
      Two-way data binding <br/>
      v-model -> formulários
    </div>

      <br><br>
    <div>
      <label>Nome</label> <br>
    <input 
        v-model="name"
        type="text"
     > <br>
     {{name}}
  </div>

  <br><br>

  <div>
    <!--Outro exemplo com select -->
    <label>Sports</label> <br>
    <select v-model="sports">
    <option disabled value="">Escolha</option>
    <option value="futebol">Futebol</option>
    <option value="skate">Skate</option>
    <option value="Tenis">Tenis</option>
    </select> <br>
    {{sports}}
  </div>

  <br><br>

  <div>
     <!--Outro exemplo com Radio -->
    <label>Newsletter</label> <br>
    <input 
      v-model="newsletter"
      type="radio"
      value="Sim"
      >Sim

    <input 
      v-model="newsletter"
      type="radio"
      value="Não"
      >Não

  </div>

  <br><br>

  <div>
     <!--Outro exemplo com Checkbox -->
    <label>Contrato</label> <br>
    <input 
      v-model="contract"
      type="checkbox"
      >Aceita nossos termos?
      <br>
    {{contract}} 
  </div>

  <br><br>

  <div>
     <!--Outro exemplo com multipla-escolha -->
    <label>Cores que você mais gosta.</label> <br>
    <input 
      v-model="colors"
      type="checkbox"
      value="Rosa"
      >Rosa

    <input 
      v-model="colors"
      type="checkbox"
      value="Azul"
      >Azul <br>
      {{colors}}

  </div>

</div>

</template>

<script>
  export default {
   name: 'App',
   data(){
    return {
      name: 'Bruna Carvalho',
      sports: '',
      newsletter: '',
      contract: '',
      colors: [] //precisa ser passado em array

      }
    }
   }
</script>