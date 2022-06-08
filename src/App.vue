<template>
<img alt="vue logo" src="./assets/logo.png">
<HelloWorld msg="I am Hello World Component!"></HelloWorld>
<HomeComponent />
<InputValue />
<CheckboxRadioValue />
<Conditions />
<ForLoop />
<ChildComponent :name="name" :data="user" :getData="getData"></ChildComponent>
<hr>
<h1>Reusable Component (data passed as an loop array from App component)</h1>
<ul style="list-style:none;">
  <li v-for="item in users" :key="item">
  <Reusable :data="item" :getUserName="getUserName" />
  </li>
</ul>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import HomeComponent from './components/HomeComponent.vue'
import InputValue from "./components/InputValue.vue"
import CheckboxRadioValue from "./components/CheckboxRadioValue.vue"
import Conditions from "./components/Conditions.vue"
import ForLoop from "./components/ForLoop.vue"
import ChildComponent from "./components/ChildComponent.vue"
import Reusable from "./components/Reusable.vue"

export default {
    name: 'App',
    components: {
        HelloWorld,
        HomeComponent,
        InputValue,
        CheckboxRadioValue,
        Conditions,
        ForLoop,
        ChildComponent,
        Reusable
    },
    data(){
      return {
        name: 'Jayrajsinh Solanki',
        user:{
           name:'Jayrajsinh Solanki',
           email:'jayrajsinhsolanki.folium@gmail.com'
        },
        getData(){
           alert('function called from App component');
        },
        getUserName(data){
             alert(data)
        },
      users:[
        {name: 'john doe',email:'johndoe@mailinator.com'},
        {name: 'peter doe',email:'peterdoe@mailinator.com'},
        {name: 'willium doe',email:'willium@mailinator.com'},
        {name: 'Stella doe',email:'stella@mailinator.com'},
        {name: 'Paul doe',email:'paul@mailinator.com'},
      ]
      }
    }

}
</script>

<style>
#app {
    text-align: center;
}
</style>
