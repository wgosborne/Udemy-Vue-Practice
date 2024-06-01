<template>
    <h1>Two way binding in multiple input boxes</h1>
    <label for="soccer">Soccer</label>
    &nbsp;
    <input type="checkbox" value="soccer" v-model="selectedSports"/>
    <br />

    <label for="football">Football</label>
    &nbsp;
    <input type="checkbox" value="football" v-model="selectedSports"/>
    <br />

    <label for="swimming">Swimming</label>
    &nbsp;
    <input type="checkbox" value="swimming" v-model="selectedSports"/>
    <br />

    <label for="hockey">Hockey</label>
    &nbsp;
    <input type="checkbox" value="hockey" v-model="selectedSports"/>
    <br />

    <label for="playerName">Player Name:</label>
    &nbsp; &nbsp;
    <label for="name1">Smith</label>
    <input name="selectedPLayer" type="radio" value="Smith" v-model="selectedPlayer"/>
    &nbsp;
    <label for="name2">Wesson</label>
    <input name="selectedPlayer" type="radio" value="Wesson" v-model="selectedPlayer"/>
    <br />

    <h3>Selected Sports: {{ selectedSports }}</h3>
    <h3>Selected Player: {{ selectedPlayer }}</h3>
</template>

<script>
    export default {
        name: "input-boxes",
        data() {
            return {
                selectedSports: [],
                selectedPlayer: [],
            }
        }
    }
</script>

<style>
</style>