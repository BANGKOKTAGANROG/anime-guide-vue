<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HiMom from './components/HiMom.vue';
</script>

<template>
    <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/genres">Genres</RouterLink>
    </nav>
    <HiMom />
    <RouterView />
</template>

<style scoped>

</style>
