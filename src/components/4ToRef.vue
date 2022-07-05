<template>
  <h3>toRef example</h3>
  <p>
    Nombre: <strong>{{ person.name }}</strong>
  </p>
  <p>
    Edad: <strong>{{ age }}</strong>
  </p>
  <button @click="changeAge">Cambiar edad</button>
</template>

<script setup>
import { reactive, toRef } from 'vue'

const person = reactive({ name: 'Pablo', age: 27 })
const age = toRef(person, 'age')

const changeAge = () => {
  age.value++
}
</script>
