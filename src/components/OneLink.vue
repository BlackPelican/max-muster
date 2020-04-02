<template>
  <div id="one-link" class="flex--row">
    <span class="link">My Story</span>
    <img class="arrow" src="../img/arrow.svg" alt="Go" />
  </div>
</template>

<script>
export default {
  name: "OneLink"
};
</script>

<style scoped>
#one-link {
  justify-content: flex-start;
  align-items: center;
  cursor: pointer;
  z-index: 3;
}

#one-link:hover .arrow {
  transform: translate(2vmin);
}

.link {
  margin-right: 2vmin;
  color: var(--c-yellow);
  font-size: 4vmin;
  text-decoration: underline;
}

.arrow {
  height: 3vmin;
  transition: transform 200ms ease-in-out;
}
</style>