<template>
  <div class="slide flex staticbg">
    <img class="slide-off" src="/yung_baezos.jpg" />
    <img id="yung_relentless_logo" src="/amazon_og_logo.png" />
    <img src="/summer_night_esprit.gif" />
    <img src="/yung_baezos.jpg" />
    <img id="yung_relentless_logo" src="/amazon_og_logo.png" />
    <img src="/summer_night_esprit.gif" />
    <img src="/yung_baezos.jpg" />
    <img id="yung_relentless_logo" src="/amazon_og_logo.png" />
    <img src="/summer_night_esprit.gif" />
    <img src="/yung_baezos.jpg" />
    <img id="yung_relentless_logo" src="/amazon_og_logo.png" />
    <img src="/summer_night_esprit.gif" />
    

    <div class="absolute flex">
      <h1 class="shadow slide-right">YUNG BAEZOS YUNG BAEZOS YUNG BAEZOS YUNG BAEZOS YUNG BAEZOS YUNG BAEZOS YUNG BAEZOS YUNG BAEZOS YUNG BAEZOS</h1>
    </div>
  </div>
</template>
<style lang="scss" scoped>
h1 {
  font-size: 100px;
  z-index: 2;
  white-space: nowrap;
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
  background-image: url("/static.jpg");
}
#yung_relentless_logo {
  height: 515px;
  flex-shrink: 0;
}
</style>