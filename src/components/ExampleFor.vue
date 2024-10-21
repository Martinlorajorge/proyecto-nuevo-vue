<template>
    <div>
        <ul>
            <li v-for="country in countries" :key="country.code">{{ country.name }}</li>
        </ul>
    </div>
</template>

<script lang="ts" setup>
import {Ref, ref} from "vue";
// Esto iría en un Model
interface ICountry {
    code:string,
    name:string
}

let countries:Ref<Array<ICountry>> = ref([
    {
        code:'es',
        name:'Spain'
    },
    {
        code:'en',
        name:'England'
    },
    {
        code:'fr',
        name:'France'
    },
    {
        code:'it',
        name:'Italy'
    }
])

</script>

<style lang="scss" scoped>

</style>