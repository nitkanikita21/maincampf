<template>
  <div class=" page">
    <Hero />
    <div class="body">
      <div class="body__block">
        <h1 class="body__text">
          О нас:
        </h1>
        <div class="body__text">
          Мы чиста пажилой флэкс
        </div>
      </div>
      <div class="body__block">
        <h1 class="body__text">
          Почему мы?
        </h1>
        <div class="body__text">
          Потому что я так сказал блэт
        </div>
      </div>
      <div class="body__block">
        <h1 class="body__text">
          Как к нам зайти?
        </h1>
        <div class="body__text">
          Вот держи АЙПИ
        </div>
        <div class="body__text">
          mc.hightwink.net
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Hero from '~/components/sections/Hero'
export default {
  components: { Hero }
}
</script>
