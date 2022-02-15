<template>
  <header>
    <div id="h-center">
      <img id="logo" src="../assets/img/logo.png" alt="red olympus">

      <ul>
        <li>Nos Packs</li>
        <li>Qui sommes nous ?</li>
        <li>Hotêls</li>
        <li>Mon comptes</li>
      </ul>


      <img id="db-icon" src="../assets/img/db-icon.png">

    </div>
  </header>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/app";


header {
  position: relative;
  display: flex;
  width: 100%;

  justify-content: center;


  #h-center {
    position: relative;
    display: flex;

    height: 100px;
    width: 70%;


    justify-items: center;
    align-content: center;
    align-items: center;

    color: $color-black;

    justify-content: space-between;

    #logo {
      margin-left: 70px;
      height: 50%;
    }

    ul {
      display: flex;
      flex-direction: row;


      list-style-type: none;


      * {
        margin-left: 30px;
      }

      li{
        font-size: 12px;
        letter-spacing: 5px;
      }

    }

    #db-icon {

      margin-left: 30px;

      width: 20px;

    }
  }

}
</style>
