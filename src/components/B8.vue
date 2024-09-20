<template>
  <div>
    <h1>bai 8</h1>
    <button @click="sortData(1)">tang dan</button>
    <button  @click="sortData(2)">giam dan</button>
    <ul>
      <li v-for="item in data" :key="item">{{item}}</li>
    </ul>
  </div>
</template>

<script setup>
import { computed, ref } from 'vue';
 const data = ref([1,4,8,7,45,2,5]);
 function sortData (sort){
    if(sort==1) return data.value.sort((a,b)=>a-b)
    if (sort==2) return data.value.sort((a,b)=>b-a)
 }
</script>

<style>

</style>