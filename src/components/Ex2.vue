<script setup>
    import { ref } from 'vue'

    // Add code here
    import me from "/assets/me.png"
    import wad from "/assets/wad.png"
    const width = ref(300);
    const height = ref(200);

    // multiple attribute binding
    const imgAttrs = {
        src: me,
        width: width.value,
        height: height.value
    }

</script>

<template>

    <!-- Add code here -->
    <!-- single attribute binding -->
    <img v-bind:src="wad" v-bind:width="width" v-bind:height="height" alt="wad logo">

    <!-- multiple attribute binding -->
    <img v-bind="imgAttrs" alt="me">

</template>
