<template>
  <div class="screenshot">
    <a :href="`#${id}`">
      <img :src="url" class="screenshot__thumbnail" />
    </a>
    <a :id="id" href="#_" class="screenshot__lightbox">
      <img :src="url" />
    </a>
  </div>
</template>

<script>
let uuid = 0;

const mixin = {
  beforeCreate() {
    this.uuid = uuid.toString();
    uuid += 1;
  }
};

export default {
  name: 'Follow',
  mixins: [mixin],
  props: {
    url: {
      type: String,
      required: true
    }
  },
  data() {
    return {
      id: `screenshot-${this.uuid}`
    };
  }
};
</script>

<style lang="scss">
.screenshot {
  margin: 0.5em;
  a,
  a:hover {
    border: none;
  }
  &__thumbnail {
    display: block;
  }
  &__lightbox {
    display: none;
    position: fixed;
    z-index: 999;
    width: 100%;
    height: 100%;
    text-align: center;
    top: 0;
    left: 0;
    background: rgba(0, 0, 0, 0.8);
  }

  &__lightbox img {
    max-width: 90vw;
    max-height: 90vh;
  }

  &__lightbox:target {
    outline: none;
    display: flex;
    align-items: center;
    justify-content: center;
  }
}
</style>
