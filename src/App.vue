<script>
export default {
  data(){
    return{
      show: true,
      list:[1,2]
    }
  }
}
</script>

<template>
 
 <button @click="list.push(list.length +1)" >Add um valor no final</button>
 <button @click="list.pop()">Remover um valor do final</button>
 <button @click="list.splice(list.length/2)">Remover metade dos valores</button>

 <ul v-if="show && list.length">
  <li v-for="item in list"> {{ item }}</li>
 </ul>
</template>

<style>

</style>
