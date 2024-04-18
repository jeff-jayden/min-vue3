<template>
  <div id="app"></div>
</template>

<script setup lang="ts">
const app = document.querySelector('#app')

let state = {
  text: 'hello hyh'
}

const effect = () => {
  app.innerText = state.text
}

effect()

setTimeout(() => {
  state.text = 'hello vue3'
}, 1000)

</script>

<style scoped>

</style>