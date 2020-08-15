<template>
  <div class="slide flex staticbg">
    <div id="sean_monterrosa" class="relative frame slide-off">
      <div class="copy">
        <h1 class="shadow blink black">occupy venture capital .org</h1>
      </div>
    </div>
    <div id="agnes_chow" class="relative frame">
      <div class="copy">
        <h1 class="shadow blink uppercase">occupy venture capital .org</h1>
      </div>
    </div>
    <div id="sean_monterrosa" class="relative frame">
      <div class="copy">
        <h1 class="shadow blink black">occupy venture capital .org</h1>
      </div>
    </div>
    <div id="agnes_chow" class="relative frame">
      <div class="copy">
        <h1 class="shadow blink uppercase">occupy venture capital .org</h1>
      </div>
    </div>
    <div id="sean_monterrosa" class="relative frame">
      <div class="copy">
        <h1 class="shadow blink black">occupy venture capital .org</h1>
      </div>
    </div>
    <div id="agnes_chow" class="relative frame">
      <div class="copy">
        <h1 class="shadow blink uppercase">occupy venture capital .org</h1>
      </div>
    </div>
    <div id="sean_monterrosa" class="relative frame">
      <div class="copy">
        <h1 class="shadow blink black">occupy venture capital .org</h1>
      </div>
    </div>
    <div id="agnes_chow" class="relative frame">
      <div class="copy">
        <h1 class="shadow blink uppercase">occupy venture capital .org</h1>
      </div>
    </div>
  </div>
</template>
<style lang="scss" scoped>
h1 {
  font-size: 80px;
  z-index: 2;
}
.slide {
  @apply p-2;
  display: flex;
  align-items: center;
  justify-content: center;
  background: black;
}
.frame {
  height: 600px;
  width: 600px;
  overflow: hidden;
  padding: 7px;
  flex-shrink: 0;
  @apply flex items-center justify-center;
}
.copy {
    @apply absolute;
}
#sean_monterrosa {
    background: magenta;
}
#agnes_chow {
    background: cyan;
    margin-left: 20px;
}
.staticbg {
    background-image: url('/static.jpg');
}
</style>