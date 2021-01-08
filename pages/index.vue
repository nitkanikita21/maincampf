<template>
  <div class="">
    <Hero />
    <!--    <section class="section features">-->
    <!--      <div class="container">-->
    <!--        <div class="features__wrap&#45;&#45;center">-->
    <!--          <h2 class="section__title">-->
    <!--            HighTwink-->
    <!--          </h2>-->
    <!--          <div class="features__list features-list">-->
    <!--            <div class="features-list__item features-list__item&#45;&#45;center">-->
    <!--              <h3>-->
    <!--                Версия-->
    <!--              </h3>-->
    <!--              <h4>-->
    <!--                1.12.х - 1.16.х-->
    <!--              </h4>-->
    <!--            </div>-->
    <!--            <div class="features-list__item features-list__item&#45;&#45;center">-->
    <!--              <h3>-->
    <!--                IP-->
    <!--              </h3>-->
    <!--              <h4>-->
    <!--                mc.hightwink.net-->
    <!--              </h4>-->
    <!--            </div>-->
    <!--            <div class="features-list__item features-list__item&#45;&#45;center">-->
    <!--              <h3>-->
    <!--                Онлайн-->
    <!--              </h3>-->
    <!--              <h4>-->
    <!--                404 игрока-->
    <!--              </h4>-->
    <!--            </div>-->
    <!--          </div>-->
    <!--        </div>-->
    <!--      </div>-->
    <!--    </section>-->
    <Features />
  </div>
</template>

<script>
import Hero from '~/components/sections/Hero'
import Features from '~/components/sections/features/Features'

export default {
  components: { Hero, Features }
}
</script>
