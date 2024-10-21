<template>
    <div class="post-container">
        <PostCard/>
    </div>
</template>

<script lang="ts" setup>
    import PostCard from './PostCard.vue';
</script>


<style scope>
    .post-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        width: 100%;
        height: 100%;
        padding: 20px;
        box-sizing: border-box;
    }
</style>