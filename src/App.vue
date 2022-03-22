<template>
  <div class="app">
    <HeaderDC></HeaderDC>
    <MainDC></MainDC>
    <FooterDC></FooterDC>
  </div>
</template>

<script>
import HeaderDC from './components/HeaderDC.vue'
import MainDC from './components/MainDC.vue'
import FooterDC from './components/FooterDC.vue'

export default {
  name: 'App',
  components: {
    HeaderDC,
    MainDC,
    FooterDC
  }
}
</script>

<style lang="scss">
@import './assets/styles/style.scss'
</style>