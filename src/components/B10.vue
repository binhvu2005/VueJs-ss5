<template>
  <div>
    <h1>bai 10</h1>
    <button @click="getRandomNumber">random number</button>
    <div>{{ number }}</div>

  </div>
</template>

<script setup>
import { ref } from 'vue';
 const number = ref([])
 const getRandomNumber = () => {
   const randomNumber = Math.floor(Math.random() * 100) + 1;
   number.value.push(randomNumber);
 }
</script>

<style>

</style>