<template>
  <div id="the-wave">
    <div class="wave wave--top"></div>
    <div class="wave wave--mid"></div>
    <div class="wave wave--bottom"></div>
  </div>
</template>

<script>
export default {
  name: "TheWave"
};
</script>

<style>
#the-wave {
  position: absolute;
  overflow: hidden;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 30vmin;
}

.wave {
  height: 100%;
  width: 200%;
  position: absolute;
  background-repeat: repeat no-repeat;
  transform-origin: center bottom;
  background-position: 0 bottom;
  background-size: 50%;
}

.wave--top {
  opacity: 0.4;
  animation: moveWave 18s linear infinite;
  background-image: url("../img/wave-1.svg");
}

.wave--mid {
  opacity: 0.6;
  animation: moveWave 14s linear infinite;
  background-image: url("../img/wave-2.svg");
}

.wave--bottom {
  opacity: 1;
  animation: moveWave 10s linear infinite;
  background-image: url("../img/wave-3.svg");
  z-index: 2;
}

@keyframes moveWave {
  0% {
    transform: translateX(0) scale(1);
  }
  50% {
    transform: translateX(-25%) scale(1.2);
  }
  100% {
    transform: translateX(-50%) scale(1);
  }
}
</style>