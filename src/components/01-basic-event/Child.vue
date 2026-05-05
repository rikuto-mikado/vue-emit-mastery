<script setup>
const emit = defineEmits(['notify-parent'])

const handleClick = () => {
    emit('notify-parent')
}
</script>

<template>
    <div style="border: 1px solid #ccc; padding: 10px;">
        <h3>Child Component</h3>
        <button @click="handleClick">send a notification to the parents</button>
    </div>
</template>

<style>

</style>