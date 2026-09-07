<script setup>
    import { ref } from 'vue'

    // Add code here
    const loginType = ref("username")
    const username = ref('') // need to initialise variable so taht the value input can be accessed here.
    const email = ref('')
    
</script>

<template>
    <h1>Please select your login option</h1>
    <!-- Add/modify code in the following to have a dropdown list 
        which lets the user to select either to login with username or email -->
    <!-- the 'username' & 'email' are literal strings -->
    <select v-model="loginType">
        <option value = "username">Username login</option>
        <option value= "email">Email login</option>
    </select>
    
    <!-- the 'username' & 'email' are variables -->
    <div v-if="loginType=== 'username'">
        <label>Username</label>
        <input v-model = "username" placeholder="Enter your username">
    </div>
    <div v-else>
        <label>Email</label>
        <input v-model = "email" placeholder="Enter your email address">
    </div>
</template>


