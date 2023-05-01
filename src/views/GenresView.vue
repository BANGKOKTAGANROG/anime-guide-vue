<script setup lang="ts">
import GenrePage from '@/components/GenrePage.vue'
type Genre = {
    name: string,
    description: string,
    images: string[]
}

const genres: Genre[] = [
    {
        name: "Кодомо",
        description: "GET://https://api.myanimelist.org/genres/kodomo#description",
        images: [
            "/kodomo/1.jpg",
            "/kodomo/2.jpg",
            "/kodomo/3.jpg",
            "/kodomo/4.jpg",
            "/kodomo/5.jpg",
        ]
    },
    {
        name: "Дзёсэй",
        description: "GET://https://api.myanimelist.org/genres/josei#description",
        images: [
            "/josei/1.jpg",
            "/josei/2.jpg",
            "/josei/3.jpg",
            "/josei/4.jpg",
            "/josei/5.jpg",
        ]
    },
    {
        name: "Сэйнэн",
        description: "GET://https://api.myanimelist.org/genres/seinen#description",
        images: [
            "/seinen/1.jpg",
            "/seinen/2.jpg",
            "/seinen/3.jpg",
            "/seinen/4.jpg",
            "/seinen/5.jpg",
        ]
    },
    {
        name: "Сёдзё",
        description: "GET://https://api.myanimelist.org/genres/shoujo#description",
        images: [
            "/shoujo/1.jpg",
            "/shoujo/2.jpg",
            "/shoujo/3.jpg",
            "/shoujo/4.jpg",
            "/shoujo/5.jpg",
        ]
    },
    {
        name: "Сёнэн",
        description: "GET://https://api.myanimelist.org/genres/shounen#description",
        images: [
            "/shounen/1.jpg",
            "/shounen/2.jpg",
            "/shounen/3.jpg",
            "/shounen/4.jpg",
            "/shounen/5.jpg",
        ]
    },
] 
</script>

<template>
    <main>
        <GenrePage :genre="genres[0]" />
        <GenrePage :genre="genres[1]" />
        <GenrePage :genre="genres[2]" />
        <GenrePage :genre="genres[3]" />
        <GenrePage :genre="genres[4]" />
    </main>
</template>

<style scoped>

</style>