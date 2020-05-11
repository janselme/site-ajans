<template>
  <div class="layout" :class="{ 'sticky-header': $route.path === '/' }">
    <Header />
    <slot />
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header";
import Footer from "@/components/Footer";

export default {
  components: {
    Header,
    Footer
  }
};
</script>


<style>
@font-face {
  font-family: "Avenir Light";
  src: local("Avenir LT Std 35 Light"), local("AvenirLTStd-Light"),
    url("../assets/fonts/AvenirLTStd-Light.woff2") format("woff2"),
    url("../assets/fonts/AvenirLTStd-Light.woff") format("woff"),
    url("../assets/fonts/AvenirLTStd-Light.ttf") format("truetype");
  font-weight: 300;
  font-style: normal;
}

@font-face {
  font-family: "Brandon Grotesque Bold";
  src: url("../assets/fonts/BrandonGrotesque-Bold.woff2") format("woff2"),
    url("../assets/fonts/BrandonGrotesque-Bold.woff") format("woff"),
    url("../assets/fonts/BrandonGrotesque-Bold.ttf") format("truetype");
  font-weight: 500;
  font-style: normal;
}

* {
  box-sizing: border-box;
}

body {
  --color-base: rgb(255, 255, 255);
  --color-base-1: rgb(243, 243, 243);
  --color-contrast: rgb(11, 19, 43);
  --color-contrast-1: rgb(43, 43, 43);
  font-family: "Avenir Light", -apple-system, system-ui, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  margin: 0;
  padding: 0;
  font-size: 16px;
  background: var(--color-base);
  color: var(--color-contrast);
  transition: background 0.5s ease;
}

body.dark {
  --color-base: rgb(0, 0, 0);
  --color-base-1: rgb(43, 43, 43);
  --color-contrast: rgb(255, 255, 255);
  --color-contrast-1: rgb(243, 243, 243);
}

h1 {
  letter-spacing: -0.01em;
  font-family: "Brandon Grotesque Bold", -apple-system, system-ui,
    BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
}

.layout {
  padding: 0;
}

.layout.sticky-header {
  padding: 6rem 0 0 0;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2rem;
}

@media (min-width: 860px) {
  .container {
    padding: 0 6rem;
  }
}

a {
  color: inherit;
}

img {
  max-width: 100%;
}

.label {
  display: block;
  font-weight: 700;
  margin-bottom: 0.5rem;
}
</style>
