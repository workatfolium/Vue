<template>
<h1>Checkboxes and Radios Value</h1>
<hr>
<h3>Select Languages:</h3>

<label for="PHP">PHP</label>
<input type="checkbox" id="PHP" value="php" v-model="languages"><br>

<label for="C++">C++</label>
<input type="checkbox" id="C++" value="c++" v-model="languages"><br>

<label for="JAVA">JAVA</label>
<input type="checkbox" id="JAVA" value="java" v-model="languages"><br>

<h3>Your Selected Languages are <span style="color:red;">{{ languages }}</span>:</h3>

<hr>

<h3>Select Gender:</h3>
<input type="radio" value="Male" name="gender" id="male" v-model="gender">
<label for="male">Male</label><br>
<input type="radio" value="Female" name="gender" id="female" v-model="gender">
<label for="female">Female</label><br>

<h3>Your Selected Gender is <span style="color:red;">{{ gender }}</span>:</h3>
</template>

<script>
export default {
    name: 'CheckboxRadioValue',
    data() {
        return {
            languages: [],
            gender: "Not Selected"
        }
    },
    methods: {

    }
}
</script>
