<template>
    <div>
        <!-- se puede dejar solo los dos puntos : y eso quiere decir que es v-bind -->
        <p v-bind:class="{danger: hasError}">El mensaje se ha enviado correctamente</p>

        <p v-bind:style="{color: hasError ? 'red' : 'green'}">Aquí pruebo estilos del v-bind</p>
        <br>

        <p v-bind:style="{backgroundColor: '#ccc', color:c}">Cambio con el botón</p>
        <button v-on:click="handleClick()">Cambiar color</button>
    </div>
</template>

<script lang="ts" setup>
    import { ref } from 'vue'
    let c = ref('blue')
    const handleClick = () => {c.value = 'red'}
</script>

<!-- Aquí no estoy usando el setup coo atributo del script -->
<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    name: 'ClassBind',
    // setup() {
    //     let hasError = false;
    //     return{hasError}
    // }
    data(){return{hasError: false}}
    // data(){return{hasError: false}} es la otra forma de hacerlo en vez de usar setup
})
</script>

<style scoped>
.danger{
    color: red;
}
</style>