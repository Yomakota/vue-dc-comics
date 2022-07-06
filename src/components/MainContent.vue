<template>
    <main>
        <div class="container">
            <span>content go here</span>
        </div>
    </main>
</template>

<script>
export default {
    name: 'MainContent',
    data() {
        return {}
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
main {
    background-color: $mainContent;
    .container {
        display: flex;
        align-items: center;
        color: white;
        padding: 3em;
    }
}
</style>