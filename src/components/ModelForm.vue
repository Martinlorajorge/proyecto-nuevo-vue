<template>
    <form action="">
        <input type="text" placeholder="ingresa un texto" v-model="inputText">
        <input type="checkbox" v-model="agree"/> Acepto los términos y condiciones
        <br>
        <br>
        <select v-model="country">
            <option value="Argentina">Argentina</option>
            <option value="Brasil">Brasil</option>
            <option value="Chile">Chile</option>
        </select>
    </form>
    <h3>{{ inputText }}</h3>
</template>

<script lang="ts" setup>
    import {Ref, ref } from 'vue';
    let inputText: Ref<string> =  ref('')
    let agree: Ref<boolean> = ref(true)
    let country: Ref<string> = ref('Argentina')
</script>

<style lang="css" scoped>

</style>