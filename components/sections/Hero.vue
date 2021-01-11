<template>
  <section class="hero">
    <div class="container">
      <div class="hero__wrap">
        <h1 class="hero__name hero__item">
          HighTwink
        </h1>
        <h2 class="hero__description">
          {{ desc }}
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
    },
    desc: {
      type: String,
      default: 'Лучший СНГ сервер Minecraft'
    }
  }
}
</script>

<style scoped>

</style>
