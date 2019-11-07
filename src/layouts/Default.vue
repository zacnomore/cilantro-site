<template>
  <div class="layout">
    <slot/>
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>

h1, h2, h3, header {
  font-family: 'Amatic SC', cursive;
  text-transform: uppercase;
}

html, body {
  font-family: 'Noto Sans', sans-serif;
  font-size: 18pt;
  color: white;
}

</style>
