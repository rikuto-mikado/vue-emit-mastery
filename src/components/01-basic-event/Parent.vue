<script setup>
import { ref } from 'vue'
import Child from './Child.vue'

const message = ref('No message here')

const handleNotify = () => {
    message.value = 'received a notification from a child component ' + new Date().toLocaleTimeString()
}
</script>

<template>
    <div style="background: #f9f9f9; padding: 20px;">
        <h2>Parent Component</h2>
        <p>Status: {{ message }}</p>
        <Child @notify-parent="handleNotify" />
    </div>
</template>

<style>

</style>