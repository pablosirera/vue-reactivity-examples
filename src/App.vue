<script setup>
import NoReactivity from './components/1NoReactivity.vue'
import BasicRef from './components/2BasicRef.vue'
import BasicReactive from './components/3BasicReactive.vue'
import ToRef from './components/4ToRef.vue'
import Computed from './components/5Computed.vue'
import Watch from './components/6Watch.vue'
</script>

<template>
  <main>
    <NoReactivity />
    <hr />
    <BasicRef />
    <hr />
    <BasicReactive />
    <hr />
    <ToRef />
    <hr />
    <Computed />
    <hr />
    <Watch />
  </main>
</template>

<style>
@import './assets/base.css';
</style>
