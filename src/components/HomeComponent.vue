<template>
<h1>Personal Details</h1>
<table border="1" cellspacing="5" cellpadding="5" align="center">
    <thead>
        <tr>
            <th>Name</th>
            <th>Email</th>
            <th>Mobile</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td>{{ getData().name }}</td>  
            <td>{{ getData().email }}</td>
            <td>+91{{ getData().mobile }}</td>
        </tr>
    </tbody>
</table>
<hr>
</template>

<script>
export default {
    name: 'HomeComponent',
    data() {
      return {
         email : 'johndoe@mailinator.com',
         name  : 'John Doe'
      } 
    },
    methods: {
        getData() {
            return {
                name : this.name,
                email: this.email,
                mobile: 6355637919,
            }
        }

    }
}
</script>
