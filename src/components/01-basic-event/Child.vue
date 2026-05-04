<script setup>
const emit = defineEmits(['notify-parent'])

const handleClick = () => {
    emit('notify-parent')
}
</script>

<template>

</template>

<style>

</style>