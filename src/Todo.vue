<script>
export default {
    data(){
        return{

        }
    }
}
</script>

<template>
    <div class="container">
        <div class="addContainer">
          <p id="title">Adicione Sua Tarefa</p>
          <input type="text" placeholder="Oque você vai fazer?"> 
          <button class="btn" >Adicionar</button>
          <button class="btn" >Mostrar</button>
         </div>
    </div>

    <div class="taskContainer">
            <h1>teste</h1>
        </div>
</template>

<style>
.container {
    background: #fff;
    width: 100%;
    margin: 120px auto;
    padding: 25px;
    border-radius: 5px;
    display: flex;
    align-items: center;
    justify-content: center;
}
#title{
    font-size: 40px;
    margin-right: 60px;
}

.addContainer{
    padding: 1rem;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-content: center;
}
.btn{
    width: 120px;
    height: 40px;
    margin: 10px;
}
.taskContainer{
    display: flex;
    justify-content: space-between;
    background-color: rgb(255, 255, 255);
}

</style>