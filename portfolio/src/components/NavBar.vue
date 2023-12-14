<template>
    <v-app-bar app color="#111111" dark flat class="px-8">
        <v-btn icon>
            <v-icon color="#A7121B">fas fa-dragon</v-icon>
        </v-btn>
        <v-space></v-space>
        <v-btn text @click="scroll('home')">Home</v-btn>
        <v-btn text @click="scroll('skills')">Skills</v-btn>
        <v-btn text @click="scroll('experience')">Experience</v-btn>
        <v-btn text @click="scroll('education')">Education</v-btn>
        <v-btn text @click="scroll('project')">Project</v-btn>
        <v-btn text @click="scroll('about')">About</v-btn>
        <v-btn text @click="scroll('contact')">Contact</v-btn>
    </v-app-bar>
</template>

<script>
    export default {
        methods: {
            scroll(refName) {
                const element = document.getElementById(refName);
                element.scrollIntoView({behavior: "smooth"});
            }
        },
    }
</script>

<style>

</style>