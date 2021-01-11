<template>
  <header class="header">
    <div class="container">
      <div class="header__wrap">
        <div class="header__logo">
          <nuxt-link to="/">
            <img alt="High twink" :src="require('~/assets/img/logo.png')">
          </nuxt-link>
          <h2 class="header_logo">
            HIGHTWINK
          </h2>
        </div>

        <nav class="header__nav header-nav">
          <nuxt-link to="/donate">
            <button class="header-nav__item button">
              Донат
            </button>
          </nuxt-link>
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
