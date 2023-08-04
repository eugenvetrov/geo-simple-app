<script setup>
    import { ref } from 'vue'
    const message = ref('')
</script>

<template>
    <input v-model="message" placeholder="напиши что-нибудь">
    <p>{{ message }} Введенно сообщение</p>
</template>