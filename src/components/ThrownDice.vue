<template>
    <div>
        <button @click="throwDice">Throw Dice</button>
    </div>
    <div>
        <table>
            <tr>
                <td>{{ input1 }}</td>
                <td>{{ input2 }}</td>
                <td>{{ input3 }}</td>
                <td>{{ input4 }}</td>
                <td>{{ input5 }}</td>
            </tr>
        </table>
    </div>
</template>
<script setup>
import {ref, reactive} from 'vue';
let dice = ref([]);
const throwDice = () => {
    let dice = [];
    for (let i = 0; i < 5; i++) {
        let randomNumber = Math.floor(Math.random() * 6 + 1);
        dice.push(randomNumber);
    }
    console.log(dice);
};
const props = defineProps([]);
</script>
<style scoped></style>
