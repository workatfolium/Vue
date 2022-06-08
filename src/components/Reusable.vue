<template>
<div style="background-color:aquamarine;"> 
    <h4>Name : {{ data.name }}  <button v-on:click="getUserName(data.name)">Alert Name</button> | Email : {{ data.email }} <button v-on:click="getUserName(data.email)">Alert Email</button></h4>
</div>
</template>

<script>
export default {
    name : "Reusable",
    props:{
        data:Object,
        getUserName:Function
    }
}
</script>