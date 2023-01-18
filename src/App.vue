<script setup>
import Todo from './Todo.vue';
</script>

<template>

  <main>
    
    <Todo/>

  </main>

</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: Roboto;
  font-size: 25px;
  color: rgb(8, 8, 8);
}
main{
    width: 100%;
    height: 100vh;
    padding: 10px;
    background-color: black;
}

</style>
