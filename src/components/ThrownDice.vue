<template>
    <button @click="throwDice">Throw Dice</button>
</template>
<script setup>
const dice = defineModel();
const emit = defineEmits(['start']);

const throwDice = () => {
    dice.value.length = 0;

    for (let i = 0; i < 5; i++) {
        let randomNumber = Math.floor(Math.random() * 6 + 1);
        dice.value.push(randomNumber);
    }

    emit('start', 'cool');
};
</script>
<style scoped></style>
