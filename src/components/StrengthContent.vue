<template>
  <section class="section-strength">
    <div class="container">
      <h2 class="section-title" v-html="settings.strength_subtitle" />
      <div class="section-columns">
        <div class="colum">
          <h3 class="column-title">Écoute</h3>
          <p class="column-text">
            <strong>Nous prenons le temps de nous rencontrer</strong> pour mieux nous connaître,
            <strong>comprendre votre projet</strong>et trouver ensemble une solution adaptée à vos objectifs et
            votre budget.
          </p>
        </div>
        <div class="colum">
          <h3 class="column-title">Expérience</h3>
          <p class="column-text">
            Après plus de 15 ans à « bafouer » les codes du
            <strong>Web</strong> et du
            <strong>Marketing</strong> en agence ou chez l’éditeur, nous avons décider de rectifier le tir. Parce
            que
            <strong>la qualité</strong>, c’est un pré-requis.
          </p>
        </div>
        <div class="colum">
          <h3 class="column-title">Accompagnement</h3>
          <p class="column-text">
            <strong>Votre site est en ligne, bravo !</strong> Ce fut un plaisir. Oui, mais non.
            Qu’il s’agisse de
            <strong>formation</strong>, communication
            <strong>emailing</strong>, sur les
            <strong>réseaux sociaux</strong> ou de
            <strong>maintenance</strong>, nous restons à vos côtés.
          </p>
        </div>
      </div>
    </div>
  </section>
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

<style>
.hero {
  text-align: center;
  width: 480px;
  max-width: 100%;
  margin: 0 auto;
  padding: 4rem 0 8rem 0;
}

.hero-title {
  font-size: 3rem;
  font-weight: 700;
  padding: 0;
  margin: 0 0 2rem 0;
}
.hero-title p,
.hero-subtitle p {
  margin: 0;
  padding: 0;
}
.hero-subtitle {
  font-size: 1.15em;
  font-weight: 400;
  line-height: 1.68;
  padding: 0;
  margin: 0;
  opacity: 0.6;
}
</style>
