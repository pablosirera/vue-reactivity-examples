<template>
  <h3>watch and watchEffect example</h3>
  <p>
    Nombre: <strong>{{ name }}</strong>
  </p>
  <button @click="changeName">Cambiar nombre</button>
</template>

<script setup>
import { ref, watch, watchEffect } from 'vue'

const name = ref('Pablo')

// ejecuta nada más abrir componente y cada vez que cambien sus dependencias
watchEffect(() => console.log('watchEffect => ', name.value))

// ejecuta cuando cambie su dependencia
watch(name, (current, prev) => {
  console.log(`watch => current: ${current} prev: ${prev}`)
})

const changeName = () => {
  name.value = 'Luis'
}
</script>
