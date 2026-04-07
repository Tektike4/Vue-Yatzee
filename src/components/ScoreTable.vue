<template>
    {{ dice }}
</template>
<script setup>
import {ref, reactive} from 'vue';
const dice = defineModel();
</script>
<style scoped></style>
