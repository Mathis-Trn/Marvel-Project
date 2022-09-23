<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheHeros from './components/TheHeros.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/Marvel_Logo.svg.png" width="300" height="100" />

    <div class="wrapper">
      <HelloWorld msg="Projet Marvel !" />
    </div>
  </header>

  <main>
    <TheHeros />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

</style>
