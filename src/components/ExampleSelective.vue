<template>
    <div>
        <!-- Se puede usar v_show pero esto lo pinta en el DOM y se puede ver cuando se inspecciona mejor usar el v-if porque solo va a pintar lo que se valida no las dos opciones -->
        <h1 v-if="age >= 18">Eres mayor de edad</h1>
        <h1 v-else>Eres menor de edad</h1>
    </div>
</template>

<script lang="ts" setup>
    let age = 10
</script>

<style lang="scss" scoped>

</style>