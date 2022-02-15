<template>
  <body>
  <div id="bg"></div>
  <header>

    <ul>
      <li>Home</li>
      <li>About</li>
      <li>Toto</li>
    </ul>

  </header>


  </body>
</template>

<script lang="ts">
export default {
  name: "Home"
}
</script>

<style lang="scss" scoped>

body {
  #bg {
    background-image: url("../assets/img/Mars11.jpg");

  }

  header {


    ul {
      position: fixed;
      justify-self: center;

      display: flex;
      flex-direction: row;
      width: 70%;
    }
  }

}
</style>
