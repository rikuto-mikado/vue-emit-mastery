<script setup>
import { ref } from 'vue';

const emit = defineEmits(['submit-text'])
const inputText = ref('')

const sendToParent = () => {
    if (!inputText.value.trim()) {
        alert('Please enter something!')
        return
    }
    emit('submit-text', inputText.value)
    inputText.value = ''
}
</script>

<template>
  <div style="border: 1px solid #42b983; padding: 10px;">
    <h3>Child (Data Sender)</h3>
    <input v-model="inputText" placeholder="Please enter something here" />
    <button @click="sendToParent">send a notification to the parents</button>
  </div>
</template>

<style>

</style>