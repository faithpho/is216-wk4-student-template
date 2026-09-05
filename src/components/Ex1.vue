<script setup>
    import { ref } from 'vue'

    // Add code here
    // challenge: use array  
    const message = ref("Choose your favorite fruit:")
    const fruits = ref(["apple", "orange", "peach"])
</script>

<template>
    {{ message }} 
   
    <label v-for="fruit in fruits" :key="fruit"> 
        <input type="radio" name="fruit" :value="fruit"> 
        {{ fruit }} 
    </label> 
    
</template>

<style scoped>
</style>
