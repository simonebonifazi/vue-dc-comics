<template>
  <div id="app">
    <MyHeader />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue'

export default {
  name: 'dc-comics',
  components: {
    MyHeader
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
#app {
  font-family: "Segoe UI", "Open Sans", Helvetica, sans-serif;
}

img {
  height: auto;
  max-width: 100%;
}

ul {
  list-style-type: none;
}
</style>
