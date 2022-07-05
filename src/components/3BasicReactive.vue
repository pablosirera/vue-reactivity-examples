<template>
  <h3>Basic reactive example</h3>
  <p>
    Nombre: <strong>{{ person.name }}</strong>
  </p>
  <button @click="changeName">Cambiar nombre</button>
</template>

<script setup>
import { reactive } from 'vue'

const person = reactive({ name: 'Pablo', age: 27 })

const changeName = () => {
  person.name = 'Luis'
}
</script>
