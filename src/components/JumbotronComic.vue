<template>
  <div class="jumbotron">
    <img src="../assets/img/jumbotron.jpg" alt="">
  </div>
</template>

<script>
export default {
    name:"JumbotronComic",
}
</script>

<style lang="scss" scoped>

    .jumbotron{
        height: 300px;
        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
        }
    }
</style>