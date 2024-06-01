<template>
    <div>
        <h1 id="pages3">pages</h1>
        <ul>
            <li v-for="program in technology" :key="program">
                {{ program }}
            </li>
        </ul>
        <br />
        <ul>
           <li v-for="data in users" v-bind:key="data.name">
                {{ data.name }}
           </li> 
        </ul>
    </div>
</template>
<script>
export default {
    name: "for-loop-practice",
    data() {
        return {
            technology: ["php", "javascript", "c#", "c++"],
            users: [{name: "wags", job: "dev"},
                {name: "joe", job: "barista"}
            ]
        }
    }
}
</script>
<style>
    
</style>