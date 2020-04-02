<template>
  <nav id="the-nav">
    <ul class="nav flex--row">
      <li v-for="(li, i) in lis" :key="i" class="nav__li">{{li}}</li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "TheNav",
  data: () => {
    return {
      lis: ["About", "Blog", "Contact"]
    };
  }
};
</script>

<style scoped>
.nav {
  justify-content: space-between;
  font-size: var(--fs-mid);
  color: var(--c-greydark);
  font-weight: 600;
}

.nav__li {
  cursor: pointer;
  transition: color 200ms ease-in-out;
}

.nav__li:hover {
  color: var(--c-greybright);
}
</style>