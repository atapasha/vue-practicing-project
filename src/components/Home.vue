<template>
<h1>Home Component</h1>
<ul>
<li v-for="item in users" :key="item">
<User  :data="item"/>
 </li>

</ul>

  </template>

<script>
 import User from './User.vue'
export default {
    name: "Home",
    components: {
         User
    },
  
data(){

    return {

        it:1,
        users:[
            {name:'ata',email:'saman@gmail.com'},
            {name:'sam',email:'saman@gmail.com'},
            {name:'ban',email:'saman@gmail.com'},
            {name:'non',email:'saman@gmail.com'}
        ]
    }
}
 

}
</script>

<style scoped>
h1 {
    color: orange
}
</style>
