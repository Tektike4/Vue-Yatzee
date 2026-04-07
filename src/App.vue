<template>
    <ThrownDice />
</template>
<script setup>
import {ref, reactive} from 'vue';
import ThrownDice from './components/ThrownDice.vue';
const dice = ref('');
const handleDice = newDice => {
    dice.value = newDice;
};
const tableMaker = dice;
</script>
<style scoped></style>
