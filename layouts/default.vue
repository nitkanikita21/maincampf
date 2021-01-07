<template>
  <div>
    <Header />
    <Sidebar />
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
import Header from '~/components/layout/Header'
import Sidebar from '~/components/layout/Sidebar'
import Footer from '~/components/layout/Footer'
export default {
  components: {
    Header,
    Sidebar,
    Footer
  }
}
</script>
