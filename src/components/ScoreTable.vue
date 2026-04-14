<template>
    {{ dice }}
    <table>
        <tr>
            <th>Upper Section</th>
            <th>How to Score</th>
            <th>Game #1</th>
            <th>Game #2</th>
            <th>Game #3</th>
            <th>Game #4</th>
            <th>Game #5</th>
        </tr>
        <tr>
            <td>Ones</td>
            <td>Count and add only ones</td>
            <td>{{ diceOfAKind }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Two's</td>
            <td>Count and add only two's</td>
            <td>{{ diceOfAKind }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Three's</td>
            <td>Count and add only three's</td>
            <td>{{ diceOfAKind }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Fours</td>
            <td>Count and add only fours</td>
            <td>{{ fourOfAKind }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Five's</td>
            <td>Count and add only Five's</td>
            <td>{{ diceOfAKind }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Sixes</td>
            <td>Count and add only sixes</td>
            <td>{{ diceOfAKind }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Toal Score</td>
            <td>-></td>
            <td>{{ upperTotalScore }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Bonus If total score is 63 or over</td>
            <td>Score 35</td>
            <td>0</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Total of Upper Section</td>
            <td>-></td>
            <td>{{ upperTotalScore }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <th>Lower Section</th>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>3 of a kind</td>
            <td>Add total of all dice</td>
            <td>{{ threeKind }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>4 of a kind</td>
            <td>Add total of all dice</td>
            <td>{{ fourKind }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Full House</td>
            <td>Score 25</td>
            <td>{{ fullHouse }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Small Straight</td>
            <td>Score 30</td>
            <td>{{ smallStraight }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Large Straight</td>
            <td>Score 40</td>
            <td>{{ largeStraight }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Yahtzee</td>
            <td>Score 50</td>
            <td>{{ Yahtzee }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Chance</td>
            <td>Add total of all Dice</td>
            <td>{{ upperTotalScore }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Yahtzee Bonus</td>
            <td>Score 100 per bonus</td>
            <td>0</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Total of Lower Section</td>
            <td>-></td>
            <td>{{ lowerTotalScore }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Total of Upper Section</td>
            <td>-></td>
            <td>{{ upperTotalScore }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
        <tr>
            <td>Grand Total</td>
            <td>-></td>
            <td>{{ grandTotal }}</td>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
    </table>
</template>
<script setup>
import {ref, reactive, computed} from 'vue';
const dice = defineModel();

const diceOfAKind = computed(() => {
    for (let I = 1; i < 7; i++) {}
});
</script>
<style scoped></style>
