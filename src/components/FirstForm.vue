<script setup>
    import { ref } from 'vue'
    const message = ref('')
</script>

<template>
    <input v-model="message" placeholder="отредактируй меня">
    <p>Введённое сообщение: {{ message }}</p>
</template>