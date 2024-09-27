<script setup>
  import MyHello from './components/MyHello.vue'
  import CompApiMyHello from './components/CompApiMyHello.vue'
</script>

<template>
  <header>
  </header>
  <div>
    <h1>Ya sdelal'</h1>
    <h2>no ne vseou</h2>
    <p>Ewe tekst prosto tekst ewe bolshe teksta chtobibilo naglyadnee vidno perehod stroki v obichnom rejime. NY vot otlichno.</p>
  </div>
  <MyHello />
  <CompApiMyHello />
</template>

<style scoped>
  div h1, h2, p {
    font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    margin-left: 5%;
    max-width: 90%;
  }
</style>
