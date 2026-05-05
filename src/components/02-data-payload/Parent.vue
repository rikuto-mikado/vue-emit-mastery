<script setup>
import { ref } from 'vue'
import Child from './Child.vue'

const receivedData = ref('No message was received')

const handleData = (val) => {
    receivedData.value = val
}
</script>

<template>
  <div style="background: #e6f7ff; padding: 20px;">
    <h3>Parent (Data Receiver)</h3>
    <p>Data from child: <strong>{{ receivedData }}</strong></p>

    <Child @submit-text="handleData" />
  </div>
</template>

<style>

</style>