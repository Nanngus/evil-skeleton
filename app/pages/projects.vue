<script setup lang="ts">
    const project1 = {
        title: "Raccoon",
        desc: "Eating Grapes With His Little Hands",
        imagePath: "/images/content/default.png"
    };
</script>
<template>
    <Header>Projects</Header>
    <div class="layout">
        <NavBar />
        <main>
            <Project 
            :title="project1.title"
            :desc="project1.desc"
            :imagePath="project1.imagePath"
            />
        </main>
    </div>
    <Footer />
</template>
<style>
    @import url("~/assets/css/default.css");
    @import url("~/assets/css/layout.css");
</style>