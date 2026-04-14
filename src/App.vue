<script setup>
const buildId = import.meta.env.VITE_BUILD_ID ?? 'local'
const today = new Date().toLocaleDateString('fr-FR')
</script>
<template>
<header>
<p>Nom : Antonin Hotte</p>
<p>Date : {{ today }}</p>
<p>Build : {{ buildId }}</p>
</header>
</template>
<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: black;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

p {
  color: black;
  font-size: 1.5rem;
}
</style>
