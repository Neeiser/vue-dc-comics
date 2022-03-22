<template>
  <div class="app">
    <HeaderDC></HeaderDC>
    <MainDC></MainDC>
    <PreFooterDC></PreFooterDC>
    <FooterDC></FooterDC>
    <FooterSocialDC></FooterSocialDC>
  </div>
</template>

<script>
import HeaderDC from './components/HeaderDC.vue'
import MainDC from './components/MainDC.vue'
import PreFooterDC from './components/PreFooterDC.vue'
import FooterDC from './components/FooterDC.vue'
import FooterSocialDC from './components/FooterSocialDC.vue'

export default {
  name: 'App',
  components: {
    HeaderDC,
    MainDC,
    PreFooterDC,
    FooterDC,
    FooterSocialDC
  }
}
</script>

<style lang="scss">
@import './assets/styles/style.scss'
</style>