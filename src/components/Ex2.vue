<script setup>
    import { ref } from 'vue'

    // Add code here
    import me from "/assets/me.png"
    const width = ref(300);
    const height = ref(200);

</script>

<template>

    <!-- Add code here -->
     <img v-bind:src="me" v-bind:width="width" v-bind:height="height">
   
</template>
