<template>
  <div class="slide flex flex-col md:flex-row staticbg">
    <div id="sean_monterrosa" class="relative frame">
      <img id="nasdaq_something_wrong" src="/nasdaq_something_wrong.png" />
    </div>
  </div>
</template>
<script>
export default {
  mounted() {
    setTimeout(function () {
      setInterval(function () {
        console.log("tick");
      }, 1000);
    }, 200);
  },
  data() {},
};
</script>
<style lang="scss" scoped>
h1 {
  font-size: 50px;
  z-index: 2;
}
.slide {
  @apply p-2;
  background: black;
}
.copy {
  @apply absolute;
}
#sean_monterrosa {
  background: magenta;
  .copy {
    bottom: 270px;
    left: 0;
  }
  img {
    @apply absolute;
    top: 0;
    left: 0;

    min-height: 100%;
    min-width: 100%;
    max-width: none;
  }
}

img {
  max-width: none !important;
  animation: nasdaq 12s infinite linear;
}
.staticbg {
  background-image: url("/static.jpg");
}
@keyframes nasdaq {
  0% {
    width: 1000px;
    filter: saturate(500%);
  }
  20% {
    transform: translateX(-200px) rotate(10deg);
  }
  100% {
    width: 2500px;
    filter: saturate(0);
    transform: translateY(-1500px) rotate(10deg);
  }
}
</style>