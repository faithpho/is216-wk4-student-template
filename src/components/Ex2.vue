<script setup>
    import { ref } from 'vue'

    // Add code here
    import me from "/assets/me.png"
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
    <img v-bind:src="me" v-bind:width="width" v-bind:height="height">

    <!-- multiple attribute binding -->
    <img v-bind="imgAttrs">

</template>
