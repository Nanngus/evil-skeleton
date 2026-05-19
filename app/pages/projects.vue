<script setup lang="ts">
    const project1 = {
        title: "Evil Skeleton",
        desc: `This very site! This is my portfolio site. 
                It is meant to be a showcase of my projects, experiences, skills, and personality. 
                I am having fun working on it, and am using it to enhance my experience with web development and the Nuxt framework.`,
        imagePath: "/images/content/evilskeleton.png"
    };
    const project2 = {
        title: "Natebook",
        desc: `This is a website that a small team and I made for PRO150 Web-based Software Projects. 
                It was made in about four weeks.
                It was a mock social media website with a fun twist. 
                The site has a rule that everyone posting on it must follow. 
                If anyone disobeys this rule, their account is immediately deleted.
                We used Nuxt, Vue, and Postgres for this assignment and it was a blast to learn them.`,
        imagePath: "/images/content/natebook.png"
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
            <Project 
            :title="project2.title"
            :desc="project2.desc"
            :imagePath="project2.imagePath"
            />
        </main>
    </div>
    <Footer />
</template>
<style>
    @import url("~/assets/css/default.css");
    @import url("~/assets/css/layout.css");
</style>