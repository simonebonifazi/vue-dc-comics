<template>
  <div class="bg">
    <MyHeader />
    <MainContent />
    <FooterTop />
    <FooterBottom />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MainContent from './components/MainContent.vue'
import FooterTop from './components/FooterTop.vue'
import FooterBottom from './components/FooterBottom.vue'

export default {
  name: 'dc-comics',
  components: {
    MyHeader,
    MainContent,
    FooterTop,
    FooterBottom,
  },
}
</script>

<style lang="scss">
@import "./assets/sass/style.scss";
</style>
