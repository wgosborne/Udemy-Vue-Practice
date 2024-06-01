<template>
    <div>
        <h1>child component</h1>
        <p>{{ name }}</p>
        <p>{{ user.name }}</p>
    </div>
    <button v-on:click="passdata()">
        Call the FUNCTION!!
    </button>
</template>
<script>
export default {
    name: "child-component",
    props: {
        name: String,
        user: Object,
        passdata: Function,
    }

}
</script>
<style>
    
</style>