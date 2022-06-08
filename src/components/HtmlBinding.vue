<template>
    <hr>
    <div v-html="name + email + table">
    </div>
</template>

<script>
export default {
    name: 'HtmlBinding',
    data(){
        return{
            name : '<h3>Jayrajsinh Solanki</h3>',
            email : '<h4>jayrajsinhsolanki.folium@gmail.com</h4>',
            table : '<table border=1 align=center><thead><tr><th>Name</th><th>Email</th></tr></thead><tbody><tr><td>Jayrajsinh Solanki</td><td>jayrajsinhsolanki.folium@gmail.com</td></tr></tbody></table>'
        }
    }
}
</script>