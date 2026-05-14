<template>
  <div class="button">
    <button @click="addOne">点我加1</button>
    <button @click="subOne">点我减1</button>
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
