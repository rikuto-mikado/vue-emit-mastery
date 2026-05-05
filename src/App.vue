<script setup>
import BasicEmitParent from './components/01-basic-event/Parent.vue'
import DataEmitParent from './components/02-data-payload/Parent.vue'
</script>

<template>
  <div class="container">
    <h1>Vue Emit Practice</h1>
    <hr>
    <h2 style="color: blue;">Step 1: Basic Emit</h2>
    <BasicEmitParent />

    <h2 style="color: blue;">Step 2: Data Payload Emit</h2>
    <DataEmitParent />
  </div>
</template>

<style scoped>
.container {
  padding: 20px;
  font-family: sans-serif;
}
</style>