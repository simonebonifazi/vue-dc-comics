<template>
  <div id="app">
    <MyLayout />
  </div>
</template>

<script>
import MyLayout from './components/MyLayout.vue'

export default {
  name: 'dc-comics',
  components: {
    MyLayout
  }
}
</script>

<style lang="scss">
//Reset
* {
  font-family: "Segoe UI", "Open Sans", Helvetica, sans-serif;
}

//Generics
#app {
  font-family: "Segoe UI", "Open Sans", Helvetica, sans-serif;
}
</style>
