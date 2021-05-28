<template>
  <div class="container">
    <div>
      <div class="about">
        <div class="about__description">
          A game as beautiful and unpredictable as life. Navigate what fate
          throws at you and explore what a life well lived can mean in this
          minimalist roguelite role playing life simulation. Life is wild and
          then you die – a thousand times over.
        </div>
      </div>

      <div class="section">
        <Buy />
      </div>

      <!-- <div class="trailer">
        <div class="iframe-container">
          <iframe
            width="560"
            height="315"
            src="https://www.youtube-nocookie.com/embed/47SFM1lvpq4"
            frameborder="0"
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
      </div> -->

      <!-- <div class="screenshots">
        <h2>Screenshots</h2>
        <div class="screenshots__container">
          <Screenshot url="/img/Core-Defense-Screenshot-1.png" />
          <Screenshot url="/img/Core-Defense-Screenshot-2.png" />
          <Screenshot url="/img/Core-Defense-Screenshot-3.png" />
          <Screenshot url="/img/Core-Defense-Screenshot-4.png" />
          <Screenshot url="/img/Core-Defense-Screenshot-5.png" />
          <Screenshot url="/img/Core-Defense-Screenshot-6.png" />
          <Screenshot url="/img/Core-Defense-Screenshot-7.png" />
          <Screenshot url="/img/Core-Defense-Screenshot-8.png" />
          <Screenshot url="/img/Core-Defense-Screenshot-9.png" />
          <Screenshot url="/img/Core-Defense-Screenshot-10.png" />
          <Screenshot url="/img/Core-Defense-Screenshot-11.png" />
          <Screenshot url="/img/Core-Defense-Screenshot-12.png" />
        </div>
      </div> -->

      <div class="section">
        <h2>Follow</h2>
        <Follow />
      </div>

      <div class="section">
        <h2>Quick Facts</h2>
        <QuickFacts />
      </div>

      <div class="section">
        <h2>Newsletter</h2>
        <Subscription />
      </div>
    </div>
  </div>
</template>

<script>
import Buy from '~/components/Buy.vue';
import Follow from '~/components/Follow.vue';
import QuickFacts from '~/components/QuickFacts.vue';
// import Screenshot from '~/components/Screenshot.vue';
import Subscription from '~/components/Subscription.vue';

export default {
  components: {
    Buy,
    Follow,
    QuickFacts,
    // Screenshot,
    Subscription,
  },
  head() {
    return {
      title: 'Core Defense',
    };
  },
};
</script>

<style lang="scss">
.about {
  width: 80vw;
  max-width: 520px;
  margin: 0 auto 40px auto;

  &__description {
    text-align: justify;
    margin: 1em 0;
    font-size: 24px;
    color: #dbdbdb;
  }
}

.iframe-container {
  position: relative;
  overflow: hidden;
  width: 100%;
  padding-top: 56.25%;

  iframe {
    position: absolute;
    top: 0;
    left: 0;
    bottom: 0;
    right: 0;
    width: 100%;
    height: 100%;
  }
}

.screenshots {
  max-width: 960px;
  margin: 80px auto;
  &__container {
    display: flex;
    flex-wrap: wrap;
    .screenshot {
      flex: 1 0 200px;
    }
  }
}

.section {
  max-width: 640px;
  margin: 60px auto;
  h2 {
    text-align: center;
    margin-bottom: 0.5em;
  }
}

.newsletter {
  margin: 80px auto;
  &__info {
    font-size: 0.8em;
    color: #aaa;
  }
}

.footer {
  margin: 4em 0 2em 0;
}
</style>
