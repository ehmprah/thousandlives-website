<template>
  <nav>
    <ul class="navigation">
      <li><a href="/">Home</a></li>
      <li><a href="/presskit">Presskit</a></li>
      <li><a href="/imprint">Imprint</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Navigation',
};
</script>

<style lang="scss">
ul.navigation {
  padding: 0;
  list-style-type: none;
  text-align: center;
  li {
    display: inline;
    margin: 0.5em;
  }
}
</style>
