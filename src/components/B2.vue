<template>
    <div>
      <h1>bai 2</h1>
      <button @click="change">{{(isShow)? "hien" : "an"}}</button>
    </div>
  </template>
  
  <script setup>
  import { ref } from "vue";
  const isShow = ref(true);
  
  const change = () => {
      isShow.value =!isShow.value;
  
  };
  

  </script>
  
  <style>
  
  </style>