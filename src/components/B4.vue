<template>
  <div>
    <h1>Bai 4</h1>
    <button @click="change1">an</button>
    <button @click="change2">hien</button>
    <p v-show="show">Hello World!</p>
    
  </div>
</template>

<script setup>
import { ref } from 'vue';
  const show = ref(false);

  const change1 = () => {
    show.value = false;
  };

  const change2 = () => {
    show.value = true;
  };
</script>

<style>

</style>