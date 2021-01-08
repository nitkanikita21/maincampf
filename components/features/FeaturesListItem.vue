<template>
  <div class="features-list__item features-list-item">
    <div class="features-list-item__icon">
      <img :src="img">
    </div>

    <div class="features-list-item__features features-list-item-features">
      <h3 class="features-list-item-features__title">
        {{ title }}
      </h3>
      <p class="features-list-item-features__desc">
        {{ desc }}
      </p>
    </div>
  </div>
</template>
<script>
export default {
  name: 'ListItem',
  props: {
    img: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    desc: {
      type: String,
      required: true
    }
  }
}
</script>
