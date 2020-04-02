<template>
  <ul id="the-socials" class="flex--row">
    <li>
      <img class="social" src="../img/github.svg" alt="Github" />
    </li>
    <li>
      <img class="social" src="../img/instagram.svg" alt="Insta" />
    </li>
    <li>
      <img class="social" src="../img/linkedin.svg" alt="linkedin" />
    </li>
  </ul>
</template>

<script>
export default {
  name: "TheSocials"
};
</script>

<style>
#the-socials {
  width: 20vmin;
  justify-content: space-between;
  z-index: 1;
}

.social {
  height: 4vmin;
}
</style>