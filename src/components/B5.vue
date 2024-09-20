<template>
  <div>
    <h1>bai 5</h1>
    <p>cac so trong mang la so chan</p>
    <ul v-for="item in array" :key="item">
      <li  v-if="item % 2 == 0">
       {{ item }}
      </li>
    </ul>

  </div>
</template>

<script setup>
const array = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17]
</script>

<style>

</style>