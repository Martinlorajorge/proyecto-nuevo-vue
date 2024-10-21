<template>
    <div>
        <h3>{{ counter }}</h3>
        <button @click="increment">Incrementar</button>
    </div>
</template>

<script lang="ts" setup>
import { Ref ,ref } from 'vue'
        let counter:Ref = ref(0)
        const increment = ():void => {
            counter.value++
        }
</script>

<style lang="scss" scoped>

</style>