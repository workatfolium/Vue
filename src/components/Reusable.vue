<template>
<div style="background-color:aquamarine;"> 
    <h4>Name : {{ data.name }}</h4>
    <h4>Email : {{ data.email }}</h4>
</div>
</template>

<script>
export default {
    name : "Reusable",
    props:{
        data:Object
    }
}
</script>