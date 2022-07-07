<template>
    <div class="thumb">
        <img :src="thumbInfo.thumb" :alt="thumbInfo.type">
    </div>
</template>

<script>
export default {
    name: "ThumbComic",
    props: {
        thumbInfo: Object
    }
}
</script>

<style lang="scss" scoped>

    .thumb{
        width: calc((100% / 6) - 10px);
        margin: 5px;
    }

</style>