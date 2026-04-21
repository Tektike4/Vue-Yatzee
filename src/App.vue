<template>
    <ThrownDice @start="frequency" v-model="dice" />
    <br />
    <table v-for="dos in dice">
        {{ dos }}
    </table>
    <br />
    <ScoreTable v-model="freqArray" />
</template>

<script setup>
import {ref} from 'vue';
import ThrownDice from './components/ThrownDice.vue';
import ScoreTable from './components/ScoreTable.vue';

const dice = ref([]);

const freqArray = ref([]);

const frequency = () => {
    for (let i = 1; i < 7; i++) {
        const amountInArray = dice.value.filter(num => num === i);
        freqArray.value[i - 1] = amountInArray.length;
    }
    console.log(freqArray.value);
};
</script>

<style scoped></style>
