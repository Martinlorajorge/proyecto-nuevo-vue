<template>
    <div>
        <h3>{{ counter }}</h3>
        <button @click="incrementar">Incrementar</button>
    </div>
</template>

<script lang="ts">
    import { defineComponent } from 'vue';
    export default defineComponent({
        name: 'CounterOption',
        components: { },
        data() {
            let counter = 0;
            return {counter}
        },
        methods: {
            incrementar() {
                this.counter++;
            }
        }
    })
</script>

<style lang="scss" scoped>

</style>