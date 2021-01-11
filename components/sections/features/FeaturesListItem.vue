<template>
  <div class="features-list__item">
    <div class=" features-list-item">
      <div class="features-list-item__icon">
        <img :src="img" :alt="title">
      </div>

      <div class="features-list-item__features features-list-item-features">
        <h3 class="features-list-item-features__title">
          {{ title }}
        </h3>
        <div class="features-list-item-features__desc">
          {{ desc }}
        </div>
      </div>
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
