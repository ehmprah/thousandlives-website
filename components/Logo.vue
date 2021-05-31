<template>
  <div class="logo">
    <a href="/" class="logo__inner">THOU<br />SAND<br />LIVES</a>
  </div>
</template>

<script>
export default {
  name: 'Logo',
};
</script>

<style lang="scss" scoped>
.logo {
  text-align: center;
  margin: 2em 0;

  &__inner {
    color: #dbdbdb;
    display: inline-block;
    text-align: center;
    font-size: 80px;
    line-height: 1em;
    font-family: 'Spectral', serif;
    font-weight: 300;
    padding: 0.15em 0.175em 0.1em;
    border: 0.04em solid;
    text-shadow: 0 0 0.05em #000;
    box-shadow: 0 0 0.05em #000, inset 0 0 0.05em #000;
  }
}
</style>
