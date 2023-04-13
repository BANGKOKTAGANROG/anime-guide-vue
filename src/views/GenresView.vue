<script setup lang="ts">

</script>

<template>
    <main>
        <div class="wrapper" id="base-grid">
            <div>images</div>
            <div>genre desc</div>
            <div class="title">
                <div id="title">
                    genre title
                </div>
                <div class="cross">
                    cross
                </div>
            </div>
            <div class="controls">
                <div class="wrapper" id="controls">
                    <div class="arrow">arrow</div>
                    <div class="arrow">reverse arrow</div>
                </div>
            </div>
        </div>
    </main>
</template>

<style scoped>
.wrapper {
    height: 100%;
    width: 100%;
    background-color: var(--border);
    display: grid;
    gap: 1px;
}

.wrapper > * {
    background-color: var(--bg);
}

#base-grid {
    grid-template-columns: 2fr 1fr;
    grid-template-rows: 2fr 1fr;
}

#base-grid > *{
    display: grid;
    place-content: center;
}

.title {
    display: flex !important;
    justify-content: space-between !important;
    align-items: center !important;
    padding: 3rem;
}

.controls {
    display: block !important;
}

#controls {
    grid-template-columns: repeat(2, 1fr);
}

.arrow {
    display: grid;
    place-content: center;
}
</style>