<template>
    <div class="thumb">
        <a href="#">
            <img :src="thumbInfo.thumb" :alt="thumbInfo.series">
            <span>{{ thumbInfo.series }}</span>
        </a>
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
.thumb {
    width: calc((100% / 6) - 20px);
    margin: 0 10px;
    height: 150px;
    img {
        height: 100%;
        object-fit: cover;
        object-position: top;
        margin: 20px 0;
    }
    a{
        color: white;
        text-transform: uppercase;
        font-size: 12px;
    }
}
</style>