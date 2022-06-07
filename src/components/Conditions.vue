<template>
<hr>
<h1>Conditions</h1>
<button v-if="show" style="color:green;">True</button>
<button style="color:red;" v-else>False</button>&nbsp;&nbsp;
<button v-on:click="show=!show" style="color:blue;">Switch</button>
</template>

<script>
export default {
    name: "Conditions",
    data() {
        return {
            show: true
        }
    }
}
</script>
