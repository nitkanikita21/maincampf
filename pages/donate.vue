<template>
  <div class="">
    <Hero :img="require('~/assets/img/hero_bg2.jpg')" />
    <div class="body">
      <div class="body__headers body__line">
        <div class="body__block body__headers">
          <h1>
            Поддержи нас!
          </h1>
          <h2>
            При покупке доната ты получаешь много плюшек!
          </h2>
        </div>
        <div class="body__block body__headers">
          <h1>
            Пару кликов и всё!
          </h1>
          <h2>
            Донат у тебя на сервере!
          </h2>
        </div>
      </div>
      <div class="body__donate_list">
        <button class="button">
          Button
        </button>
        <button class="button">
          Button
        </button>
        <button class="button">
          Button
        </button>
        <button class="button">
          Button
        </button>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
.back {
  background: url(https://icdn2.digitaltrends.com/image/digitaltrends/continuum-best-minecraft-shaders2.jpg) no-repeat 50%;
}
.head {
  height: 300px;
  padding: 45px;
  &__name {
    padding: 5px;
    color: white;
  }
}
.body {
  align-items: center;
  background: rgb(157, 157, 157);
  background: white;

  &__text {
    font-family: "Roboto", sans-serif;
  }

  &__block {
    padding: 35px;
  }
  button{
      margin: 10px;
      padding: 25px;
  }
  &__donate_list{
    padding: 50px;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
  }
  &__headers{
      display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
  }
  &__line{
      border-bottom: 3px dashed rgb(177, 177, 177);
  }
  h1 , h2 , h3{
      padding: 5px;
      font-family: "Roboto", sans-serif;
  }
}

</style>
<script>
import Hero from '~/components/sections/Hero'
export default {
  components: {
    Hero
  }
}
</script>
