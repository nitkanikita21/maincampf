<template>
  <div
    class="features-list__item donate-box"
  >
    <img :src="require('~/assets/img/hero_bg2.jpg')" class="donate-box__img">
    <div class="donate-box__wrap donate-box-wrap">
      <h2 :class="'donate-box__title'">
        {{ name }}
      </h2>
      <div class="donate-box__desc">
        {{ desc }}
      </div>
    </div>
    <div class="donate-box-price donate-box__price">
      <div class="donate-box-price-box">
        <div class="donate-box-price-box__text">
          {{ price }} ₽
        </div>
        <a class="button" href="https://hightwink.trademc.org/">
          Купить
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DonateBox',
  props: {
    color: {
      type: String,
      default: ' '
    },
    name: {
      type: String,
      default: 'Название доната'
    },
    desc: {
      type: String,
      default: 'Описание доната'
    },
    price: {
      type: Number,
      required: true
    }

  }
}
</script>
