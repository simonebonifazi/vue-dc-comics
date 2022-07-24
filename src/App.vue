<template>
  <div class="bg">
    <MyHeader />
    <MainContent />
    <FooterTop />
    <section id="footer-bottom">

    </section>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'
import MainContent from './components/MainContent.vue'
import FooterTop from './components/FooterTop.vue'

export default {
  name: 'dc-comics',
  components: {
    MyHeader,
    MainContent,
    FooterTop
  }
}
</script>

<style lang="scss">
//layout
div {
  border: 2px dashed blue;
  min-height: 80px;
}

section {
  border: 2px solid green;
  min-height: 250px;
}

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
}

.d-flex {
  display: flex;
}

.bg {
  background-color: #1c1c1c;
}
</style>
