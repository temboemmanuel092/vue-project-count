<script setup>
  import {ref} from "vue "
  const count = ref(10);

  const addToCount = () =>{
    count.value = count.value + 1; 
  }
  const subtractCount = () =>{
    count.value = count.value - 1; 
  }
</script>

<template>
  <main>
    <div>
      <h4>The current count</h4>  
      <h1>
        {{ count }}
      </h1>  
      <button @click="subtractCount()">-</button>
      <button @click="addToCount()">+</button>
        
  </div>
  </main>
</template>

<style scoped>
  main {
    background-color: aliceblue;
    width: 100vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;


  }
  main {
    text-align: center ;
  }
</style>