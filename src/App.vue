<template>
    <div>
        <ThrownDice :input1="tableMaker" />
    </div>
    <div>
        <ThrownDice v-model="dice.value"></ThrownDice>
    </div>
</template>
<script setup>
import {ref, reactive} from 'vue';
import ThrownDice from './components/ThrownDice.vue';
const dice = ref([]);
const tableMaker = dice;
</script>
<style scoped></style>
