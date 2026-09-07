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
<!-- 
if never put :value this is how it will show in backend
<input type="radio" name="fruit">
<input type="radio" name="fruit">
<input type="radio" name="fruit"> -->
<style scoped>
</style>
