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
      <img :src="img" alt="background">
    </div>
  </section>
</template>

<script>
export default {
  name: 'Hero',
  props: {
    img: {
      type: String,
      default: require('~/assets/img/hero-bg.jpg')
    }
  }
}
</script>

<style scoped>

</style>
