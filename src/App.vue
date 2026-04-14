<template>
    <ThrownDice v-model="dice" />
    <br />
    <table v-for="dos in dice">
        {{ dos }}
    </table>
    <br />
    <ScoreTable></ScoreTable>
    <button @click="frequency">test</button>
</template>

<script setup>
import {ref} from 'vue';
import ThrownDice from './components/ThrownDice.vue';
import ScoreTable from './components/ScoreTable.vue';

const dice = ref([]);

const freqObj = {};

const frequency = () => {
    for (let i = 0; i < 6; i++) {
        const amountInArray = dice.value.filter(num => num === i + 1);
        freqObj[i + 1] = amountInArray.length;
    }
    console.log(freqObj);
};
</script>

<style scoped></style>
