<template>
  <div id="app">
    <TheHeader />
  </div>
</template>

<script>
import TheHeader from "./components/TheHeader.vue";

export default {
  name: "App",
  components: {
    TheHeader
  },
  computed: {
    scrollbarWidth() {
      return window.innerWidth - document.documentElement.clientWidth;
    }
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Sen:300,400,600,700&display=swap");

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

:root {
  --c-dark: #333646;
  --c-darker: #252734;
  --c-greydark: #888874; /* 666874 */
  --c-greybright: #ebebec;
  --c-yellow: #ffc25c;
  --fs-big: 13vmin;
  --fs-mid: 5.5vmin;
  --fs-small: 2.6vmin;
}

html,
body {
  position: relative;
  font-family: "Sen";
}

#app {
  display: flex;
  flex-direction: column;
  width: 100%;
}

ul {
  list-style-type: none;
}

.flex--row {
  display: flex;
  flex-direction: row;
}

.flex--column {
  display: flex;
  flex-direction: column;
}

.flex--center {
  display: flex;
  justify-content: center;
  align-items: center;
}

.wrapper--category {
  justify-content: flex-start;
}

.title--category {
  font-size: var(--fs-small);
  color: var(--c-greydark);
  letter-spacing: 0.2vmin;
  margin-bottom: 2vmin;
}

.title--paragraph {
  font-size: var(--fs-mid);
}

.paragraph {
  font-size: var(--fs-small);
  color: var(--c-greydark);
  line-height: 2;
  z-index: 1;
}
</style>
