<template>
<h1>Text , Email & Password Fields</h1>
<hr>
<input type="text" placeholder="Enter Name" v-model="name">&nbsp;
<input type="email" placeholder="Enter Email" v-model="email">&nbsp;
<input type="password" placeholder="Enter Password" v-model="password"><br><br>
<button v-on:click="getData()">Get Data</button>
<hr>
</template>

<script>
export default {
    name: 'InputValue',
    data() {
        return {
            name: null,
            email: null,
            password: null
        }
    },
    methods: {
        getData() {
            alert('Name:' + this.name + ' Email:' + this.email + ' Password:' + this.password + ' ');
        }
    }
}
</script>

<style>
input {
    padding: 5px;
}
</style>
