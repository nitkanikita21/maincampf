<template>
  <section class="hero">
    <div class="container">
      <div class="hero__wrap">
        <h1 class="hero__name">
          HighTwink
        </h1>
        <h2 class="hero__description">
          Лучший СНГ сервер Minecraft
        </h2>
      </div>
    </div>
    <div class="hero__bg">
      <img :src="require('~/assets/img/hero-bg.jpg')" alt="background">
    </div>
  </section>
</template>

<script>
export default {
  name: 'Hero'
}
</script>

<style scoped>

</style>
