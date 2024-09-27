<template>
  <p> A eto - Zveruga komponent</p>
  <p> Znachenie zverugstva seichas - {{ count }}</p>
  <button @click="increment">Dobavit' zverugstva na +1</button>
</template>

<script>
  export default {
    data() {
        return {
            count: 0
        }
    },

    methods: {
        increment() {
            this.count++
        }
    }
  }
</script>

<style scoped>

  p {
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    margin-left: 5%;
    max-width: 90%;
    background-color: rgb(189, 201, 223);
  }

  button {
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    margin-left: 5%;
    background-color: rgb(230, 84, 17);
    font-size: 18px;
    border-radius: 30px;
    color:rgb(255, 255, 255);
    padding: 5px 10px;
    cursor: pointer
  }

  button:active {
    box-shadow: 2px 5px rgba(13, 45, 13, 0.3);
    margin-top: 3px;
    margin-bottom: -3px;
  }
   
  button:hover {
    background-color: rgb(13, 233, 13);
  }

</style>
