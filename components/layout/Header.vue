<template>
  <header class="header">
    <div class="container">
      <div class="header__wrap">
        <nuxt-link to="/" class="header__logo">
          <img alt="High twink" :src="require('~/assets/img/Logo.svg')">
        </nuxt-link>
        <nav class="header__nav header-nav">
          <a href="https://vk.com/hightwink" class="header-nav__item button" target="_blank"> VK </a>
          <a href="https://discord.com/invite/WvWyh9N" class="header-nav__item button" target="_blank"> DICKSCORD </a>
        </nav>
        <div class="header__menu-open" @click="toggleSidebar">
          <img :src="require('~/assets/img/openMenu.svg')" alt="Open Menu">
        </div>
      </div>
    </div>
  </header>
</template>

<script>

import { mapActions } from 'vuex'

export default {
  name: 'Header',
  methods: {
    ...mapActions({
      toggleSidebar: 'toggleSidebar'
    })
  }
}
</script>

<style scoped>

</style>
