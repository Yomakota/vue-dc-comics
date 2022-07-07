<template>
  <section class="jumbotron">
   <div class="banner">
      <img src="../assets/img/jumbotron.jpg" alt="">
    </div>
  </section>
</template>

<script>
export default {
  name: "JumbotronComic",
}
</script>

<style lang="scss" scoped>
.banner {
  height: 300px;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: top;
  }
}
</style>