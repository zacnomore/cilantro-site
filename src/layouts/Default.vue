<template>
  <div class="layout">
    <slot/>
  </div>
</template>

<style>

/* amatic-sc-regular - latin */
@font-face {
  font-family: 'Amatic SC';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: local('Amatic SC Regular'), local('AmaticSC-Regular'),
       url('../assets/fonts/amatic-sc-v13-latin-regular.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('../assets/fonts/amatic-sc-v13-latin-regular.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

/* noto-sans-regular - latin */
@font-face {
  font-family: 'Noto Sans';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: local('Noto Sans'), local('NotoSans'),
       url('../assets/fonts/noto-sans-v9-latin-regular.woff2') format('woff2'), /* Chrome 26+, Opera 23+, Firefox 39+ */
       url('../assets/fonts/noto-sans-v9-latin-regular.woff') format('woff'); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}

h1, h2, h3, header {
  font-family: 'Amatic SC', cursive;
}

html, body {
  font-family: 'Noto Sans', sans-serif;
  font-size: 14px;
  color: white;
}

p, li {
  line-height: 180%;
}

</style>
