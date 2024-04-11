<script setup>
import { ref } from 'vue'
const name = import.meta.env.VITE_NAME
defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>
  <div class="card">
    {{ name }}
    <button type="button" @click="count++">count is {{ count }}</button>
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
