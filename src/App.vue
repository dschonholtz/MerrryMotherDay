<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style lang="scss">
  // FONT
  $default-font-size: 1.6rem;
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
  }
  @font-face {
    font-family: 'antonine_personal_useregular';
    src: url('./assets/fonts/antonine_personal_use-webfont.woff2') format('woff2'),
         url('./assets/fonts/antonine_personal_use-webfont.woff') format('woff');
    font-weight: normal;
    font-style: normal;
  }
</style>
