<template>
    <h1>Two way binding</h1>
    <input type="text" placeholder="Add a Number" v-model="count"/>
    <h3>{{ count }}</h3>
</template>

<script>
    export default {
        name: "pages-one",
        data() {
            return {
                count: 0,
            }
        }
    }
</script>

<style>
</style>