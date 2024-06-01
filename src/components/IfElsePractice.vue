<template>
    <div>
        <h1 id="pages2" v-if="display">Display</h1>
        <h1 id="pages2" v-else>Show</h1>
        <button v-on:click="display = !display">Click Me!!!!</button>
    </div>
    <Child name="wags" :user="array" :passdata="getData"/>
</template>
<script>
import Child from './child';

export default {
    name: "if-else-condition",
    data() {
        return{
            display: true,
            show: true,
            array: {name: "swagtron"}
        };
    },
    methods: {
        getData() {
            alert("methods");
        }
    },
    components: {Child}
};
</script>
<style>
    
</style>