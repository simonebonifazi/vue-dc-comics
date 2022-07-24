<template>

  <header>
    <div class="container d-flex ">
      <figure>

        <img src="../assets/img/dc-logo.png" alt="dc-logo">
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
  data() {
    return {
      links: [
        {
          text: 'Characters',
          url: '#',
          current: false,
        },
        {
          text: 'Comics',
          url: '#',
          current: true,
        },
        {
          text: 'Movies',
          url: '#',
          current: false,
        },
        {
          text: 'TV',
          url: '#',
          current: false,
        },
        {
          text: 'Games',
          url: '#',
          current: false,
        },
        {
          text: 'Collectibles',
          url: '#',
          current: false,
        },
        {
          text: 'Videos',
          url: '#',
          current: false,
        },
        {
          text: 'Fans',
          url: '#',
          current: false,
        },
        {
          text: 'News',
          url: '#',
          current: false,
        },
        {
          text: 'Shop',
          url: '#',
          current: false,
        },
      ]

    }
  }

}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header {
  background-color: #fff;
  margin-top: 15px;
}

.container {
  justify-content: space-between;
  align-items: center;
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

img {
  padding: 15px 0;

  width: 80px
}
</style>
