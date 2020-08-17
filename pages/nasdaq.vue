<template>
  <div class="staticbg">
    <div id="sean_monterrosa" class="relative frame">
      <img src="/nasdaq_automated_quotations.png" />
    </div>
    <div id="agnes_chow" class="relative frame">
      <img src="/wallenberg_investor_ab.png" />
    </div>
  </div>
</template>
<style lang="scss" scoped>
h1 {
  font-size: 50px;
  z-index: 2;
}
.slide {
  @apply p-2;
  background: black;
}
.frame {
  height: auto;
  width: 600px;
  overflow: hidden;
  padding: 7px;
  @apply flex items-center justify-center;
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
}
#agnes_chow {
  background: cyan;
  margin-left: 20px;
  .copy {
    margin-top: 20px;
  }
}
.staticbg {
  background-image: url("/static.jpg");
  height: 5000px;

}
img {
    width: 50vw;
}
#agnes_chow,
#sean_monterrosa {
    animation: investor 15s infinite linear;
}
@keyframes investor {
    to {
        transform: rotate(90deg) translate(1500px);
    }
}
</style>
