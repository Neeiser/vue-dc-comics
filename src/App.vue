<template>
  <div class="app">
    <HeaderDC></HeaderDC>
    <HeroDC></HeroDC>
    <MainDC></MainDC>
    <PreFooterDC></PreFooterDC>
    <FooterDC></FooterDC>
    <FooterSocialDC></FooterSocialDC>
  </div>
</template>

<script>
import HeaderDC from './components/HeaderDC.vue'
import HeroDC from './components/HeroDC.vue'
import MainDC from './components/MainDC.vue'
import PreFooterDC from './components/PreFooterDC.vue'
import FooterDC from './components/FooterDC.vue'
import FooterSocialDC from './components/FooterSocialDC.vue'

export default {
  name: 'App',
  components: {
    HeaderDC,
    HeroDC,
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