<template>
    <hr>
    <h1>{{ msg }}</h1>
    <button v-on:click="toggleAlert()">Click me to show alert box!</button><br><br>
    <button v-on:click="increment()"> + </button>&nbsp;
    <span>{{ count }}</span>&nbsp;
    <button v-on:click="decrement()"> - </button>
    <hr>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
     return {
        toggleAlert(){
            alert('hello world!');
        },
        count : 0,
        increment(){
           this.count = this.count+1;
        },
        decrement(){
           this.count = this.count-1;
        }
     }
  }
}
</script>