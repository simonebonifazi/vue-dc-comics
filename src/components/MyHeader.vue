<template>

  <header class="d-flex container">
    <figure>
      <img src="../assets/img/dc-logo.png" alt="dc-logo">
    </figure>

    <ul class="d-flex">
      <li> CHARACTERS</li>
      <li class="active"> COMICS</li>
      <li>MOVIES</li>
      <li>TV</li>
      <li>GAMES</li>
      <li>COLLECTIBLES</li>
      <li>VIDEOS</li>
      <li>FANS</li>
      <li>NEWS</li>
      <li>SHOP</li>
    </ul>

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
  justify-content: space-between;
  align-items: center;
}

.active {
  border-bottom: 2px solid #0282F9;
  color: #0282F9;
}

li {
  height: 35px;
  width: 35px;
  border: 1px dashed black;
}
</style>
