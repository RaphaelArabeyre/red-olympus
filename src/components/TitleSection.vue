<template>
  <div :class="primary? 'title-section-primary' : 'title-section-secondary' ">
    <div class="title">
      <h2>{{ title }}</h2>
      <hr>
    </div>
  </div>
</template>

<script>
export default {
  name: "TitleSection",

  props: {
    title: String,
    primary: Boolean,
  }


}
</script>

<style lang="scss" scoped>
@import "../assets/scss/app";

.title-section-primary{

  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;

  div {
    h2 {
      font-weight: 400;
      font-size: 22px;
      margin: 3px auto 0;
      text-transform: uppercase;
      letter-spacing: 3px;
    }

    hr {
      border: 0;
      align-self: center;
      position: relative;
      height: 2.6px;
      width: 70px;
      background: $color-primary;
    }
  }
}

.title-section-secondary{

  background: $color-primary;
  width: 100%;
  height: 70px;
  align-self: center;
  display: flex;
  flex-direction: column;
  align-items: center;

  justify-content: center;

  div {
    h2 {
      font-size: 22px;
      margin: 3px auto 0;
      color: $color-white;
      text-transform: uppercase;
      letter-spacing: 3px;
    }

    hr {
      align-self: center;
      position: relative;
      height: 2.6px;
      width: 70px;
      background: $color-white;
    }
    }
}


</style>
