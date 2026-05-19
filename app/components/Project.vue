<script setup lang="ts">
    defineProps<{
        title: string,
        desc: string,
        imagePath: string
    }>()
</script>

<template>
    <section class="project">
        <h3 class="proj-title">{{ title }}</h3>
        <article class="proj-desc">{{ desc }}</article>
        <img name="proj-pic" class="proj-pic" :src="imagePath" alt="Image of my project.">
    </section>
</template>

<style>
    @import url("~/assets/css/project.css");
</style>