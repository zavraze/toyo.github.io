<script setup>
import {ref} from 'vue';
  let counter = ref(0);

  function add() {
    counter.value++;
  }

  function subtract() {
    counter.value--;
  }
</script>

<template>
  <div>
    <h1>{{ counter }}</h1>
    <button @click="add()" class="add"> + </button>
    <button @click="subtract()" class="subtract"> - </button>
  </div>
</template>

<style>
  body{
    text-align: center;
    margin-top: 50px;
}

h1{
    color: rgb(0, 0, 0);
    font-size: 100px;
}

button{
    font-size: 50px;
    border: none;
    background-color: rgb(0, 0, 0);
    color: white;
    border-radius: 10px;
    padding: 5px 50px;
}

.add {
    margin-right: 5px;
}

.subtract {
    margin-left: 5px;
}

</style>