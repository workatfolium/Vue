<template>
  <img alt="vue logo" src="./assets/logo.png">
  <HelloWorld msg="I am Hello World Component!"></HelloWorld>
  <HomeComponent />
  <InputValue />
  <CheckboxRadioValue />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import HomeComponent from './components/HomeComponent.vue'
import InputValue from "./components/InputValue.vue"
import CheckboxRadioValue from "./components/CheckboxRadioValue.vue"

export default {
  name: 'App',
  components: {
    HelloWorld,
    HomeComponent,
    InputValue,
    CheckboxRadioValue
  }
}
</script>

<style>
   #app {
     text-align: center;
   }
</style>