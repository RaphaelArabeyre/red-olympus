<template>
  <div :class="primary ? 'primary':'secondary'">
    <p class="button-text">{{ text }}</p>
  </div>
</template>

<script lang="ts">
export default {
  name: 'ROButton',
  props: {
    'text': String,
    'primary': Boolean,
  },

}
</script>

<style lang="scss" scoped>
@import "../assets/scss/app";

div.primary{
  background: $color-primary;
  height: 40px;
  width: 120px;
  display: grid;
  justify-content: center;
  align-content: center;

  .button-text{
    font-size: 11px;
    color: $color-white;
  }

}

div.secondary{
  border: solid $color-secondary;
  border-width: 1px;
  height: 40px;
  width: 120px;
  display: grid;
  justify-content: center;
  align-content: center;


  .button-text{
    font-size: 11px;
    color: $color-black;
  }

}

</style>
