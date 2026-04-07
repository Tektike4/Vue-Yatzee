<template>
    <ThrownDice v-model="dice" />
    <br />
    <table v-for="dos in dice">
        {{ dos }}
    </table>
    <br />
    <ScoreTable></ScoreTable>
</template>

<script setup>
import {ref} from 'vue';
import ThrownDice from './components/ThrownDice.vue';
import ScoreTable from './components/ScoreTable.vue';

const dice = ref([]);
</script>

<style scoped></style>
