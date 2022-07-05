<template>
  <h3>Computed example</h3>
  <p>
    Nombre: <strong>{{ fullName }}</strong>
  </p>
  <button @click="changeName">Cambiar nombre</button>
</template>

<script setup>
import { computed, reactive } from 'vue'

const person = reactive({ name: 'Pablo', lastName: 'Sirera' })

const fullName = computed(() => {
  return `${person.name} ${person.lastName}`
})

const changeName = () => {
  person.name = 'Luis'
}
</script>
