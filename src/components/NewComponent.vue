<template>
    <h1>Hello! {{ 10+10 }}</h1>
    <p>my email is {{ email }}</p>
    <p>my cell is {{ cell = 78}}</p>
    <p>name: {{ getName("last") }}</p>
    <p>data: {{ getData().Email}}</p>
    <!-- example of interpolation is above -->

    <button v-on:dblclick="onClick()">click here</button>
    <h1 v-on:mousemove="getConsole()">Mouse Here</h1>
    <!-- example of events are above -->

</template>

<script>
    export default {
        name: "PAGES", //must be capital to avoid error
        data() {
            return{
                email: "abc@gmail.com",
                cell: '55-555',
            };
        },
        methods: {
            getName(name) {
                return name;
            },
            getData() {
                return {
                    Email: "abc@gmail.com",
                    Cell: +6306966451,
                }
            },
            onClick() {
                alert("i've been clicked")
            },
            getConsole() {
                console.warn('function is running')
            }
        }
    }
</script>

<style scoped>
</style>