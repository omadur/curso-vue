<template>
    <!--Recorrido de estructuras-->
    <ul>
        <li v-for="country in countries" v-bind:key="country.name">{{ country.name}}</li>
    </ul>
</template>

<script setup>
import {ref} from 'vue';

let countries = ref([
    {code: 'es', name: 'Spain'},
    {code: 'fr', name: 'Italy'},
    {code: 'col', name:'Colombia'}
])
</script>

<style scoped>

</style>