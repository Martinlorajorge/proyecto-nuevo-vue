<template>
    <div class="post-card">
        <h3>Titulo</h3>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit</p>
        <PostButton />
    </div>
</template>

<script lang="ts" setup>
    import PostButton from './PostButton.vue';

</script>

<style scoped>
    .post-card{
        background-color: #fff;
        padding: 1rem;
        border-radius: 1rem;
        box-shadow: 0 0 1rem rgba(0, 0, 0, 0.1);
        margin-bottom: 1rem;
    }
</style>