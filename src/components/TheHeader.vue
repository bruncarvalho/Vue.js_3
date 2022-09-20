<template>

<div>
      
  <h1 :class="{'title': true, 'title_home': isHome}">
    Curso Vue.js 3
  </h1>

  <p :class="pClass">
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolorem recusandae consequatur error, qui repellendus doloremque amet corrupti obcaecati esse modi saepe vel perspiciatis iusto eligendi voluptas ab nam assumenda earum!
  </p>

  <p :style="styleClass">
    Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laborum corporis inventore autem dicta nesciunt, dolor delectus voluptates quo, assumenda sint ex reiciendis quod provident dolorem, voluptas dolore molestiae temporibus. Officiis!
  </p>
      <div v-for="(obj, index) in todos"
      :key="obj.id"
      class="todos-items"
      >
      <img 
      v-if="obj.imgSrc"
      :src="obj.imgSrc">
      
        {{index}} - {{obj.title}}
</div>
    
</div>
</template>

<script>
  export default {
   name: 'App',
   data(){
    return {
      classVar: 'title',
      isHome: true,
      pClass: ['text', 'text_home' ], 
      styleClass: {'color': 'green', 'background': 'black'},
      todos: 
        [
         
  {
    "userId": 1,
    "id": 1,
    "title": "delectus aut autem",
    "completed": false,
    imgSrc: 'https://via.placeholder.com/150'
  },
  {
    "userId": 1,
    "id": 2,
    "title": "quis ut nam facilis et officia qui",
    "completed": false,
    imgSrc: 'https://via.placeholder.com/150'
  },
  {
    "userId": 1,
    "id": 3,
    "title": "fugiat veniam minus",
    "completed": false
  },
  {
    "userId": 1,
    "id": 4,
    "title": "et porro tempora",
    "completed": true
  },
  {
    "userId": 1,
    "id": 5,
    "title": "laboriosam mollitia et enim quasi adipisci quia provident illum",
    "completed": false
  }
]
      }
    }
   }
  

</script>

<style>
  .title{
    font-size: 20px;
    color: blue
  }
  .title_home{
    font-size: 40px;
    color: pink
  }
  .text{
    color: rgb(8, 109, 95)
  }
  .text_home{
    color: brown
  }

  .todos-items{
    background: black;
    margin: 0 0 5px 0;
    padding: 3px, 6px;
    color: #fff
  }
 .header{
  background: #bbb;
  color: black;
 }
</style>