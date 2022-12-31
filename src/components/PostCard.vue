<template>
    <div class="post-card">
        <h3>Título</h3>
        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Cum, iure cupiditate? Illum sunt reprehenderit
            facere incidunt. Reprehenderit fuga deleniti perferendis libero tempore. Recusandae ea repellendus
            asperiores tenetur enim omnis earum?
        </p>
        <PostBtnVue />
    </div>
</template>

<script setup>
import PostBtnVue from './PostBtn.vue';
</script>

<style scoped>
.post-card {
    border-radius: 5px;
    padding: 10px;
    margin: 5px;
    border: 1px solid #ccc;
}
</style>