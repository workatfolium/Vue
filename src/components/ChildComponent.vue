<template>
    <h1>Child Component (data comes from App Component)</h1>
    <p>{{ name }}</p>
    <p>{{ data.email }}</p>
    <button v-on:click="getData()">click here</button>
</template>


<script>
export default {
    name : "ChildComponent",
    props: {
       name:String,
       data:Object,
       getData:Function
    }
}
</script>