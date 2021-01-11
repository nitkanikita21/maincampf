<template>
  <section class="section features ">
    <div class="container">
      <div class="features__wrap--center">
        <h2 class="section__title">
          Покупая донат вы:
        </h2>
        <div class="features__list features-list">
          <div
            v-for="(item, index) in text"
            :key="index"
            class="features__wrap--center features-list__item"
          >
            <h3>{{ item.title }}</h3>
            <h5 class="features__wrap--center">
              {{ item.desc }}
            </h5>
          </div>
        </div>
        <div class="features__list features-list features-list--horizontal">
          <DonateBox
            v-for="(item, index) in donates"
            :key="index"
            :name="item.name"
            :desc="item.desc"
            :color="item.color"
            :price="item.price"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import DonateBox from './DonateBox.vue'
export default {
  name: 'Features',
  components: {
    DonateBox
  },
  data () {
    return {
      text: [
        {
          title: 'Поддерживаете нас',
          desc: 'Ваша поддержка важна для нас! Как материальная, так и моральная! Каждный ваш донат даёт нам силы на улучшение наших возможностей'
        },
        {
          title: 'Получаете привелегии',
          desc: 'Отличайтесь префиксом, правами и уважением игроков на сервере! Новый донат - новые возможности'
        },
        {
          title: 'Ранний доступ к новым режимам',
          desc: 'Донатерам открывается предварительный доступ к новым режимам.'
        }
      ],
      donates: [
        {
          name: 'BRILLIANT',
          desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
          price: 600,
          color: 'blue1'
        },
        {
          name: 'RUBY',
          desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
          price: 350.00,
          color: 'red'
        },
        {
          name: 'SAPHIRE',
          desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
          price: 150.00,
          color: 'blue2'
        },
        {
          name: 'BRILLIANT',
          desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
          price: 600,
          color: 'blue1'
        },
        {
          name: 'RUBY',
          desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
          price: 350.00,
          color: 'red'
        },
        {
          name: 'SAPHIRE',
          desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.',
          price: 150.00,
          color: 'blue2'
        }

      ]
    }
  }
}
</script>
