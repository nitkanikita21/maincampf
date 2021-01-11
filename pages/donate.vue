<template>
  <div class="">
    <Hero :img="require('~/assets/img/hero_bg2.jpg')" desc="Донат - это ваша поддержка" />
    <FeaturesDonate />
  </div>
</template>

<script>
import Hero from '~/components/sections/Hero'
import FeaturesDonate from '~/components/sections/features/FeaturesDonate'

export default {
  components: { Hero, FeaturesDonate }
}
</script>
