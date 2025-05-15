<script setup>
import { ref, computed } from 'vue'
import Main from './components/Main.vue'
import Golpes from './components/Golpes.vue'
import Ferramentas from './components/Ferramentas.vue'
import NotFound from './components/NotFound.vue'
import ConsultarDadosVazados from './components/ConsultarDadosVazados.vue'

const routes = {
  '/': Main,
  '/golpes': Golpes,
  '/ferramentas': Ferramentas,
  '/consultar-dados-vazados':ConsultarDadosVazados,
  '/not-found':NotFound,
}
const currentPath = ref(window.location.hash)

window.addEventListener('hashchange', () => {
  currentPath.value = window.location.hash
})

const currentView = computed(() => {
  return routes[currentPath.value.slice(1) || '/'] || NotFound
})

</script>

<template>

    <component :is="currentView" />

 
</template>

<style scoped>

</style>
