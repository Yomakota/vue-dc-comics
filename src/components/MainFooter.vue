<template>
    <footer>
        <FooterTop />
        <FooterBottom />
    </footer>
</template>

<script>
import FooterTop from './FooterTop.vue';
import FooterBottom from './FooterBottom.vue';
export default {
    name: "MainFooter",
    components: {
        FooterTop,
        FooterBottom,
    },
    data() {
        return {

        }
    }
}
</script>

<style lang="scss" scoped>
</style>