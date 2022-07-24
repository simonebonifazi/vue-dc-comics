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
    FooterBottom
  }
}
</script>

<style lang="scss">
//Reset
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

//Generics
body {
  font-family: "Segoe UI", "Open Sans", Helvetica, sans-serif;
}

.container {
  max-width: 1080px;
  margin: 0 auto;
}


img {
  height: auto;
  max-width: 100%;
}

ul {
  list-style-type: none;
}

a {
  text-decoration: none;
  color: inherit;

  cursor: pointer;
}

.d-flex {
  display: flex;
}

body {
  background-color: #1c1c1c;
}
</style>
