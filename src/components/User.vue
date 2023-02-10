<template>
<div class="user">
    <h2>{{data.name}}</h2>
    <h2>{{data.email}}</h2>
    <button v-on:click="getA(data.name)">Allert USer Name</button>
</div>
</template>

<script>
export default {

    name: 'User',
    props: {
        data: Object
    },

    methods: {

        getA(name) {

            alert(name)
        }

    }

}
</script>

<style>
.user {

    background-color: skyblue;
    padding: 10px;
    margin-bottom: 15px;
}
</style>
