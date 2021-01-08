<template>
  <section class="section features ">
    <div class="container">
      <div class="features__wrap--center">
        <h2 class="section__title">
          Наши режимы
        </h2>
        <p class="section__desc">
          У нас не много режимов, но они смогут тебя зацепить и застаивть остаться с нами!
        </p>
        <div class="features__list features-list">
          <ListItem
            v-for="(item, index) in features"
            :key="index"
            :img="item.img"
            :title="item.title"
            :desc="item.desc"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import ListItem from '~/components/sections/features/FeaturesListItem'

export default {
  name: 'Features',
  components: { ListItem },
  data () {
    return {
      features: [
        {
          img: require('~/assets/img/games/1.jpg'),
          title: 'Creative',
          desc: 'Строй ломай и побеждай'
        }, {
          img: require('~/assets/img/games/1.jpg'),
          title: 'CastleWars',
          desc: 'Красные против синих!'
        }, {
          img: require('~/assets/img/games/1.jpg'),
          title: 'ThePit',
          desc: 'Сражайся и будь в топе!'
        }
      ]
    }
  }
}
</script>

<style scoped>

</style>
