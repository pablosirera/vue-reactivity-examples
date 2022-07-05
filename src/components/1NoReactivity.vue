<template>
  <h3>No Reactivity example</h3>
  <p>
    {{ count }}
  </p>
  <input v-model="count" type="number" />
</template>

<script setup>
const count = 0
</script>
