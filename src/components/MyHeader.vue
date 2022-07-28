<template>

  <header>
    <div class="container d-flex ">
      <figure>
        <a href="#">

          <img src="../assets/img/dc-logo.png" alt="dc-logo">
        </a>
      </figure>

      <ul class="d-flex">
        <li v-for="link in links" :key="link.text" :class="{ 'active': link.current }"> <a :href="link.url"> {{
            link.text
        }}</a></li>
      </ul>

    </div>
  </header>

</template>

<script>
export default {
  name: 'MyHeader',
    
  props:{
    links: Array,
  },

}

</script>

<style scoped lang="scss">
header {
  background-color: #fff;
  margin-top: 15px;

  .container {
    justify-content: space-between;
    align-items: center;

    img {
      padding: 15px 0;

      width: 80px
    }
  }

  .active {
    border-bottom: 2px solid #0282F9;
    color: #0282F9;
  }

  li {
    height: 35px;

    padding: 10px;

    font-size: 12px;
  }

}
</style>
