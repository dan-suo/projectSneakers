<script setup>
  import {ref} from 'vue'
  let newCount = ref(1.1);

  function newIncrement() {
    newCount.value *= newCount.value;
  }

  function updateNewCount(event) {
    newCount.value = Number(event.target.value);
  }
</script>

<template>
    <main>
        <h1>Teper' nachinaetsya cirk</h1>
        <p>i zahodit composition api, ego zverugstvo ewe silnee i typo po knopke vozvodit svoe sverugstvo v sleduywyy stepen'</p>
        <p>Seichas zverugstvo CompAPI - {{ newCount }}</p>
        <button @click="newIncrement"> Ymnojit' Zverugstvo</button>
        <p>Rewili, chto znachenie zverugstva na samom dele drugoe? Ny piwite ego suda togda sami, hozyain barin.</p>
        <input v-on:input="updateNewCount" /> 
    </main>
</template>

<style scoped>

  main {
    margin: 5% 5%;
    max-width: 90%;
    font-family:Verdana, Geneva, Tahoma, sans-serif;
  }

  button {
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    background-color: rgb(45, 67, 196);
    font-size: 18px;
    border-radius: 30px;
    color:rgb(255, 255, 255);
    padding: 5px 10px;
    cursor: pointer;
  }

  button:active {
    box-shadow: 2px 5px rgba(150, 43, 123, 0.3);
    margin-top: 3px;
    margin-bottom: -3px;
  }
   
  button:hover {
    background-color: rgb(107, 161, 182);
  }

  input {
    border: 2px solid cornflowerblue;
    border-radius: 10px;
    margin: 0 auto;
    padding: 10px 10px;
    margin: 0 25%;
  }

  h1 {
    font-size: 27px;
    text-decoration: underline;
  }
</style>