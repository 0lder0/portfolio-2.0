<script setup>
import waveGif from '../assets/images/wave.gif';
</script>

<template>
    <div class="intro-layout">
        <div class="intro-container">
            <h2>Hi, my name is</h2>
            <h1>Lilii-Ann Older</h1>
            <h2>and this is my portfolio</h2>
        </div>

        <div class="wave-container" aria-label="Animated wave illustration">
            <img :src="waveGif" alt="Animated wave" />
        </div>
    </div>
</template>