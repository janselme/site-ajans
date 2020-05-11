<template>
  <footer class="footer">
    <div class="container">
      <span v-html="settings.footer" />
      <nav class="right">
        <g-link
          class="nav__link"
          to="/mentions-legales"
        >Les mentions légales, parce que c'est obligatoire</g-link>
        <g-link class="nav__link" to="/contact">Contact</g-link>
        <g-link class="nav__link" :to="settings.link_linkedin">Linkedin</g-link>
        <g-link class="nav__link" :to="settings.link_instagram">Instagram</g-link>
      </nav>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      settings: require("../../data/theme.json")
    };
  }
};
</script>

<style scoped>
.footer {
  font-size: 0.8rem;
  padding: 6rem 0;
}
</style>
