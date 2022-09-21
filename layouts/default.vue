<template>
  <div>
    <Logo />

    <Nuxt />

    <div class="footer">
      <Navigation />
    </div>
  </div>
</template>

<style lang="scss">
@font-face {
  font-family: 'Spectral';
  font-style: normal;
  font-weight: 400;
  src: url('/fonts/spectral-v13-latin-regular.eot'); /* IE9 Compat Modes */
  src: local(''),
    url('/fonts/spectral-v13-latin-regular.eot?#iefix')
      format('embedded-opentype'),
    /* IE6-IE8 */ url('/fonts/spectral-v13-latin-regular.woff2') format('woff2'),
    /* Super Modern Browsers */ url('/fonts/spectral-v13-latin-regular.woff')
      format('woff'),
    /* Modern Browsers */ url('/fonts/spectral-v13-latin-regular.ttf')
      format('truetype'),
    /* Safari, Android, iOS */
      url('/fonts/spectral-v13-latin-regular.svg#Spectral') format('svg'); /* Legacy iOS */
}

html {
  font-family: 'Spectral', sans-serif;
  font-size: 20px;
  color: #dbdbdb;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  padding: 20px;

  &::after {
    content: '';
    width: 150vmax;
    height: 150vmax;
    position: fixed;
    left: 50%;
    top: 50%;
    z-index: -1;
    background: linear-gradient(0deg, #46203c, #162b3c);
    animation: rotate 15s ease-in-out infinite;
  }
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}

a,
a:visited {
  color: #9953df;
  text-decoration: none;
  border-bottom: 1px solid;
}

img {
  max-width: 100%;
  height: auto;
}

@keyframes rotate {
  0% {
    transform: translate(-50%, -50%) rotate(0);
  }
  100% {
    transform: translate(-50%, -50%) rotate(360deg);
  }
}
</style>
