<script setup>
import { ref } from 'vue';

const hoveredIcon = ref(null);

const showText = (icon) => {
  hoveredIcon.value = icon;
};

const hideText = () => {
  hoveredIcon.value = null;
};

</script>

<template>
    <nav class="nav-container">
    <div class="navbar">
      <ul>
        <li @mouseenter="showText('home')" @mouseleave="hideText">
          <a href="#home"><img src="../assets/nav-icons/home.svg" /></a>
          <div v-if="hoveredIcon === 'home'" class="navbar-text">Home</div>
        </li>

        <li @mouseenter="showText('about')" @mouseleave="hideText">
          <a href="#about"><img src="../assets/nav-icons/about.svg" /></a>
          <div v-if="hoveredIcon === 'about'" class="navbar-text">About Me</div>
        </li>

        <li @mouseenter="showText('skills')" @mouseleave="hideText">
          <a href="#skills"><img src="../assets/nav-icons/skills.svg" /></a>
          <div v-if="hoveredIcon === 'skills'" class="navbar-text">Skills</div>
        </li>

        <li @mouseenter="showText('projects')" @mouseleave="hideText">
          <a href="#projects"><img src="../assets/nav-icons/projects.svg" /></a>
          <div v-if="hoveredIcon === 'projects'" class="navbar-text">Projects</div>
        </li>

        <li @mouseenter="showText('contact')" @mouseleave="hideText">
          <a href="#contact"><img src="../assets/nav-icons/contact.svg" /></a>
          <div v-if="hoveredIcon === 'contact'" class="navbar-text">Contact</div>
        </li>
      </ul>
    </div>
  </nav>
</template>

