<template>
  <h3>Basic ref example</h3>
  <p>
    {{ count }}
  </p>
  <input v-model="count" type="number" />

  <button @click="updateNumber">Poner valor a 8</button>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)

const updateNumber = () => {
  count.value = 8
}
</script>
