<template>
  <div class="home">
    <Button
    @addOne="add"
    @subOne="sub"
    />
    <Count
    :number1="number"/>
  </div>
</template>

<script setup >
import Button from "@/Button.vue"
import Count from "@/Count.vue"
import { ref } from "vue"
const number = ref(0)
const add = () => {
  number.value++

}

const sub = () => {
  number.value--

}
</script>

<style scoped>

</style>
