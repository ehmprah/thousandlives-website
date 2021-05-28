<template>
  <ul class="buy">
    <li>
      <a href="https://store.steampowered.com/app/1631360/Thousand_Lives/">
        <img src="/badges/steam.png" alt="Wishlist Thousand Lives on Steam" />
      </a>
    </li>
    <li v-if="false">
      <a
        href="https://play.google.com/store/apps/details?id=com.ehmprah.coredefense"
      >
        <img
          src="/badges/google-play.png"
          alt="Get Core Defense on Google Play"
        />
      </a>
    </li>
    <li v-if="false">
      <a href="https://apps.apple.com/us/app/core-defense/id1546364145">
        <img
          src="/badges/app-store.png"
          alt="Get Core Defense on the App Store"
        />
      </a>
    </li>

    <li v-if="false">
      <a href="https://ehmprah.itch.io/core-defense">
        <img src="/badges/itchio.png" alt="Buy Core Defense on itch.io" />
      </a>
    </li>
  </ul>
</template>

<script>
export default {
  name: 'Buy',
};
</script>

<style lang="scss">
ul.buy {
  margin: 1em auto;
  max-width: 640px;
  padding: 0;
  list-style-type: none;
  display: flex;
  justify-content: center;
  li {
    margin: 0 0.5em;
    max-width: 200px;
    a {
      display: block;
      border-bottom: none;
      transition: all 0.1s;
      &:hover {
        transform: scale(1.05);
      }
    }
    img {
      display: block;
      max-width: 100%;
      height: auto;
    }
  }
}
</style>
