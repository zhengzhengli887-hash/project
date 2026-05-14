<template>
  <div class="button">
    <button @click="addOne">点我+1</button>
    <button @click="subOne">点我-1</button>
  </div>
</template>

<script setup>
const emit = defineEmits(['addOne', 'subOne'])
const addOne = () => {
  emit('addOne')
}
const subOne = () => {
  emit('subOne')
}
</script>

<style scoped></style>
