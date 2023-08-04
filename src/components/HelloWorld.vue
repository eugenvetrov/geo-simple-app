<script setup>
import { ref } from 'vue'
import FirstForm from './FirstForm.vue'
import SecondForm from './SecondForm.vue'

const first = ref(true)

const handleFirst = () => {
  first.value = !first.value
}

</script>

<template>
  <keep-alive>
    <component v-if="first" :is="FirstForm"></component>
    <component v-else :is="SecondForm"></component>
  </keep-alive>
  <button @click="handleFirst">Переключить</button>
</template>