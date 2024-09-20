<template>
    <div>
      <h1>bai 1</h1>
      <button @click="change">hien</button>

      <p v-if="isVisible">Rikei education</p>
    </div>
  </template>
  
  <script setup>
  import { ref } from "vue";
  const isVisible = ref(true);
  
  const change = () => {
    isVisible.value =!isVisible.value;
  };
  

  </script>
  
  <style>
  
  </style>