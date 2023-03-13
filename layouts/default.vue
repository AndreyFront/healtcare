<template>
    <div class="layout wrapper-page">
        <Header />
        <NuxtPage />
        <Footer />
    </div>
</template>

<script>
import Header from '@/components/layouts/Header'
import Footer from '@/components/layouts/Footer'

export default {
  name: 'indexPage',
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">
  
</style>