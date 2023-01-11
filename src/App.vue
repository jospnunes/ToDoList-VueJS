<script>
export default {
  data(){
    return{
      show: true,
      list:[]
    }
  }
}

</script>

<template>

<div id="flex">
  <p v-if="list.length">A lista atualmente possui {{ list.length }} itens.</p>
  <p v-else> Lista Vazia!</p>
</div>

<div id="flex">
  <button @click="list.push(list.length +1)" >Add um valor no final</button>
  <button @click="list.pop()">Remover um valor do final</button>
  <button @click="list.splice(list.length/2)">Remover metade dos valores</button>
  <input v-model="textInput" placeholder="Digite algo">
  <button @click="list.push(textInput)">Add o texto ao lado na lista</button>
</div>


<div id="flex">
  <ul v-if="show && list.length">
    <li  v-for="item in list"> {{ item }}</li>
  </ul>
</div>

 
</template>

<style>
#flex{
  display: flex;
  justify-content: center;
  align-content: center;
  
}

button{
  width: 100px;
  height: 45px;
  border: 2px;
  margin: 5px;
}
button:hover{
  background-color: rgb(61, 19, 19);
}
</style>
