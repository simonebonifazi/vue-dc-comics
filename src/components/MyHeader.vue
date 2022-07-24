<template>

  <header>
    <div class="container d-flex ">
      <figure>

        <img src="../assets/img/dc-logo.png" alt="dc-logo">
      </figure>

      <ul class="d-flex">
        <li> <a href="#"> CHARACTERS</a></li>
        <li class="active"> <a href="#"> COMICS</a></li>
        <li> <a href="#"> MOVIES</a></li>
        <li> <a href="#"> TV</a></li>
        <li> <a href="#"> GAMES</a></li>
        <li> <a href="#"> COLLECTIBLES</a></li>
        <li> <a href="#"> VIDEOS</a></li>
        <li> <a href="#"> FANS</a></li>
        <li> <a href="#"> NEWS</a></li>
        <li> <a href="#"> SHOP</a></li>
      </ul>

    </div>
  </header>

</template>

<script>
export default {
  name: 'MyHeader'
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
}
</style>
