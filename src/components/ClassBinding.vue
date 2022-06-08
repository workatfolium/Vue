<template>
    <hr>
    <h1 :class="{color:toggleclass}">Class Binding</h1>
    <button v-on:click="toggleclass=!toggleclass">Toggle Class</button>
</template>

<script>
export default {
    name: 'ClassBinding',
    data(){
        return {
            toggleclass : false
        }
    }
}
</script>
<style>
.color{
    color:green;
}
</style>