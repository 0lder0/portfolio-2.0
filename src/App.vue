<script setup>
import Navigation from './components/Navigation.vue';
import Intro from './components/Intro.vue';
import About from './components/About.vue';
import Skills from './components/Skills.vue';
import Projects from './components/Projects.vue';
</script>

<template>
  <Navigation />
  <Intro id="home"/>
  <About id="about"/>
  <Skills id="skills"/>
  <Projects id="projects"/>
</template>