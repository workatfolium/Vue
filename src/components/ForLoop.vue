<template>
<hr>
<h1>For Loop in Vue</h1>
<span>(1) with one key values.</span><br>
<ul style="list-style:none;">
  <li v-for="tech in technologies" :key="tech">{{ tech }}</li>
</ul>
<hr>

<span>(2) with two key values.</span><br><br>
<table border="1" cellspacing="5" cellpadding="5" align="center">
    <thead>
        <tr>
            <th>Language</th>
            <th>Framework</th>
        </tr>
    </thead>

    <tbody>
        <tr v-for="item in languageswithframeworks" :key="item">
            <td>{{ item.language }}</td>
            <td>{{ item.frameworks }}</td>
        </tr>
    </tbody>
</table>
<hr>
</template>

<script>
export default {
    name: "ForLoop",
    data() {
        return {
            technologies:[
               'php',
               'laravel',
               'vue',
               'javascript',
               'python',
               'react'
            ],
            languageswithframeworks: [{
                    language: 'php',
                    frameworks: 'Laravel,Codeignitor,Zend,Falcon,Symphony',
                },
                {
                    language: 'javascript',
                    frameworks: 'React,Vue,Next,Nuxt,Angular',
                },
                {
                    language: 'python',
                    frameworks: 'Django',
                },
            ]
        }
    }
}
</script>
