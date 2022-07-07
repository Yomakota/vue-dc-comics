<template>
    <main>
        <MainContent />
        <MainMenu />
    </main>
</template>

<script>
import MainContent from './MainContent.vue';
import MainMenu from './MainMenu.vue';

export default {
    name: "MainDcComics",
    components: {
        MainContent,
        MainMenu,
    },
    data() {
        return {

        }
    }
}
</script>

<style>
</style>