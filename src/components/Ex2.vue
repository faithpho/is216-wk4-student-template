<script setup>
    import { ref } from 'vue'

    // Add code here
    import me from "/assets/me.png"
    const width = ref(200);
    const height = ref(200);
    const obj = ref({
        src: '/assets/me.png',
        width: 200,
        height: 200
    })
    // width : '200' also can! cos vue.js reads it as a string regardless,
    // so you put width: 200 ==> will be seen as "200"!!!
</script>

<template>

    <!-- Add code here -->
     <img v-bind:src="me" v-bind:width="width" v-bind:height="height">
     <img v-bind="obj">

   
</template>
