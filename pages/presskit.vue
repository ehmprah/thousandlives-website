<template>
  <div class="container">
    <div>
      <h1 class="title">PRESSKIT</h1>

      <div class="text">
        <div class="text__description">
          A game as beautiful and unpredictable as life. Navigate what fate
          throws at you and explore what a life well lived can mean in this
          minimalist roguelite role playing life simulation. Life is wild and
          then you die – a thousand times over.
        </div>
      </div>

      <div class="section">
        <div class="iframe-container">
          <iframe
            width="560"
            height="315"
            src="https://www.youtube-nocookie.com/embed/PIRtGEB26zI"
            frameborder="0"
            allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
      </div>

      <div class="text">
        <h2>Team</h2>
        <div class="text__description">
          Thousand Lives is the first game of emfinite studio. The
          german-french-canadian indie studio is comprised of Mario Kaiser,
          Mathias Tournier and Michael Champion and hails from Berlin and
          Vancouver.
        </div>
        <div class="text__description">
          Thousand Lives was first conceived years ago by Mario "ehmprah"
          Kaiser, who until now was busy making
          <a href="https://store.steampowered.com/app/649770/Coregrounds/"
            >Coregrounds</a
          >
          and its spin-off
          <a href="https://store.steampowered.com/app/1203360/Core_Defense/"
            >Core Defense</a
          >. But success of the latter laid the foundation to finally make this
          passion project a reality.
        </div>
      </div>

      <div class="section screenshots">
        <h2>Screenshots</h2>
        <p class="centered">
          <a href="/screenshots/thousand-lives-screenshots.zip"
            >Download as .zip</a
          >
        </p>
        <div class="screenshots__container">
          <Screenshot url="/screenshots/01.png" />
          <Screenshot url="/screenshots/02.png" />
          <Screenshot url="/screenshots/03.png" />
          <Screenshot url="/screenshots/04.png" />
          <Screenshot url="/screenshots/05.png" />
          <Screenshot url="/screenshots/06.png" />
        </div>
      </div>

      <!-- <div class="screenshots screenshots--gif">
        <h2>GIFs</h2>
        <p><a href="/gifs/Core-Defense-GIFs.zip">Download as .zip</a></p>
        <div class="screenshots__container">
          <Screenshot url="/gifs/Core-Defense-1.gif" />
          <Screenshot url="/gifs/Core-Defense-2.gif" />
          <Screenshot url="/gifs/Core-Defense-3.gif" />
          <Screenshot url="/gifs/Core-Defense-4.gif" />
          <Screenshot url="/gifs/Core-Defense-5.gif" />
          <Screenshot url="/gifs/Core-Defense-6.gif" />
          <Screenshot url="/gifs/Core-Defense-7.gif" />
          <Screenshot url="/gifs/Core-Defense-8.gif" />
          <Screenshot url="/gifs/Core-Defense-9.gif" />
          <Screenshot url="/gifs/Core-Defense-10.gif" />
          <Screenshot url="/gifs/Core-Defense-11.gif" />
          <Screenshot url="/gifs/Core-Defense-12.gif" />
        </div>
      </div> -->

      <div class="section">
        <h2>Logos</h2>
        <p class="centered">
          <a href="/logos/thousand-lives-logos.zip">Download as .zip</a>
        </p>
        <div class="logos__container">
          <Screenshot url="/logos/01.png" />
          <Screenshot url="/logos/02.png" />
          <Screenshot url="/logos/03.png" />
        </div>
      </div>

      <div class="section">
        <h2>Quick Facts</h2>
        <QuickFacts />
      </div>

      <div class="section">
        <h2>Links</h2>
        <ul class="list-inline">
          <li>
            <a href="https://store.steampowered.com/app/1631360/Thousand_Lives/"
              >Steam</a
            >
          </li>
          <li>
            <a href="https://discord.gg/YWwXW3KP9v">Discord</a>
          </li>
          <li>
            <a href="https://twitter.com/ehmprah">Twitter</a>
          </li>
        </ul>
      </div>

      <div class="section">
        <h2>Contact</h2>
        <p class="centered">
          <a href="mailto:ehmprah@gmail.com">ehmprah@gmail.com</a>
        </p>
      </div>

      <div class="section">
        <h2>Newsletter</h2>
        <Subscription />
      </div>
    </div>
  </div>
</template>

<script>
import QuickFacts from '~/components/QuickFacts.vue';
import Screenshot from '~/components/Screenshot.vue';
import Subscription from '~/components/Subscription.vue';

export default {
  components: {
    QuickFacts,
    Screenshot,
    Subscription,
  },
  head() {
    return {
      title: 'Presskit Thousand Lives',
    };
  },
};
</script>

<style lang="scss">
.title {
  margin: 1em;
  line-height: 1.5em;
  font-size: 2em;
  text-align: center;
}

.text {
  width: 80vw;
  max-width: 640px;
  margin: 0 auto 80px auto;

  &__description {
    text-align: justify;
    margin: 1em 0;
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
  &--gif {
    .screenshot {
      flex: 1 0 200px;
      height: 112px;
      overflow: hidden;
    }
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

.logos {
  &__container {
    display: flex;
    justify-content: center;
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

p.centered {
  text-align: center;
  margin-bottom: 0.5em;
}

ul.list-inline {
  list-style-type: none;
  text-align: center;

  li {
    display: inline;
    margin: 0.5em;
  }
}
</style>
