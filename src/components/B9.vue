<template>
  <div>
    <h1>bai 9</h1>
    <p>gender : {{genderRef}}</p>
    <button @click="randomGender">random gender</button>
  </div>
</template>

<script setup>
import { ref } from 'vue';
  const genders = ['nam', 'nu' ,'khac']
  const genderRef = ref('nam')

  const randomGender = () => {
    genderRef.value = genders[Math.floor(Math.random() * genders.length)]
  }
</script>

<style>

</style>