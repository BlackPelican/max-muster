<template>
  <div id="the-header">
    <div class="stars"></div>
    <div class="header__grid">
      <img class="logo" src="../img/logo.svg" alt="Logo" />
      <TheNav />
      <h1 class="title--main">Max Muster.</h1>
      <div class="wrapper--category flex--column">
        <h3 class="title--category">- Introduction</h3>
        <h2 class="title--paragraph">Product Designer und Developer, based in Entenhausen.</h2>
      </div>
      <div class="decoration"></div>

      <p
        class="paragraph"
      >Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa.</p>

      <TheSocials />
      <OneLink />
      <TheWave />
    </div>
  </div>
</template>

<script>
import TheNav from "./TheNav.vue";
import OneLink from "./OneLink.vue";
import TheWave from "./TheWave.vue";
import TheSocials from "./TheSocials.vue";

export default {
  name: "TheHeader",
  components: {
    TheNav,
    OneLink,
    TheWave,
    TheSocials
  }
};
</script>

<style scoped>
#the-header {
  height: 100vmin;
  background: linear-gradient(to bottom, transparent, var(--c-dark));
  color: var(--c-greybright);
  padding: 12vmin 30vmin;
  position: relative;
}

.header__grid {
  height: 100%;
  display: grid;
  grid-template-columns: 60% 40%;
  grid-template-rows: 25% 40% 25% 10%;
}

.logo {
  height: 8vmin;
}

.title--main {
  max-width: 6vmin;
  line-height: 1;
  font-size: var(--fs-big);
}

.decoration {
  width: 12vmin;
  background: var(--c-yellow);
  height: 1.5vmin;
}

.stars {
  background: url("../img/stars.jpg");
  background-size: contain;
  height: 100vmin;
  width: 100vmax;
  position: absolute;
  left: 0;
  top: 0;
  z-index: -1;
}
</style>