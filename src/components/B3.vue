<template>
  <div>
    <h1>Bai 3</h1>
    <p v-if="userRole=='admin'">quyen han cua ban la : {{userRole}}</p>
    <p v-else-if="userRole=='guest'">quyen han cua ban la : {{userRole}}</p>
    <p v-else-if="userRole=='user'">quyen han cua ban la : {{userRole}}</p>


  </div>
</template>

<script setup>
 const userRole = "user"
</script>

<style>

</style>