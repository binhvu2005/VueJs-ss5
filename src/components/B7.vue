<template>
    <div>
    
        <h1>Bài 7</h1>
    
        <button :class="{ active: activeIndex === 1 }" @click="setActiveIndex(1)">
    
            Button 1
    
          </button>
    
        <button :class="{ active: activeIndex === 2 }" @click="setActiveIndex(2)">
    
            Button 2
    
          </button>
    
        <button :class="{ active: activeIndex === 3 }" @click="setActiveIndex(3)">
    
            Button 3
    
          </button>
    
    </div>
</template>
  
<script setup>
import { ref } from 'vue'

const activeIndex = ref(1)

const setActiveIndex = (index) => {
    activeIndex.value = index
}
</script>
  
<style scoped>
.active {
    background-color: red;
    color: #fff;
}
</style>
  