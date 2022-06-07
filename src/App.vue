<template>
  <img alt="vue logo" src="./assets/logo.png">
  <HelloWorld msg="Hello World Component!"></HelloWorld>
  <HomeComponent />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import HomeComponent from './components/HomeComponent.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    HomeComponent
  }
}
</script>

<style>
#app{
  text-align: center;
}
</style>

