<template>
  <div>
    <Header />
    <Sidebar />
    <Nuxt />
  </div>
</template>

<script>
import Header from '~/components/layout/Header'
import Sidebar from '~/components/layout/Sidebar'
export default {
  components: {
    Header,
    Sidebar
  }
}
</script>
