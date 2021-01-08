<template>
  <div class=" page">
    <Hero />
    <section class="section features">
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
              :img="require('~/assets/img/games/1.jpg')"
              :title="'Creative'"
              :desc="'Строй ломай и побеждай'"
            />
            <ListItem
              :img="require('~/assets/img/games/1.jpg')"
              :title="'CastleWars'"
              :desc="'Красные против синих!'"
            />
            <ListItem
              :img="require('~/assets/img/games/1.jpg')"
              :title="'ThePit'"
              :desc="'Сражайся и будь в топе!'"
            />
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import Hero from '~/components/sections/Hero'
import ListItem from '~/components/features/FeaturesListItem'
export default {
  components: { Hero, ListItem }
}
</script>
