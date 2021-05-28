<template>
  <div class="container">
    <div class="imprint">
      <h1 class="imprint__heading">Imprint</h1>
      <div class="imprint__section">
        ehmprah<br />
        Mario Kaiser<br />
        Graudenzer Str. 17<br />10243 Berlin
      </div>

      <div class="imprint__section">
        Email: <a href="mailto:ehmprah@gmail.com">ehmprah@gmail.com</a>
      </div>

      <div class="imprint__section">
        Google Play and the Google Play logo are trademarks of Google LLC. The
        App Store and Apple Logo are trademarks of Apple Inc., registered in the
        U.S. and other countries.
      </div>
    </div>
  </div>
</template>

<script></script>

<style lang="scss">
.imprint {
  width: 80vw;
  max-width: 480px;
  margin: 3em auto;
  text-align: center;

  &__heading {
    font-size: 2em;
    line-height: 1.5em;
    margin-bottom: 0.5em;
  }

  &__section {
    margin: 2em 0;
  }
}
</style>
