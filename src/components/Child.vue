<template>
<h2>Child Component {{name}}</h2>
<h2>Child Component {{ff}}</h2>
<button v-on:click="getd()">click konid</button>
</template>

<script>
export default {
    name: "Child",
    props:{
         // eslint-disable-next-line no-undef
         name:String,
            ff:Object,
            getd:Function
    }
}
</script>
