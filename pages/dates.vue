<template>
  <div class="slide flex staticbg">
    <div id="sean_monterrosa" class="relative frame">
      <img src="/sean.png" />
      <div class="copy">
        <h1 class="shadow">SEAN MONTERROSA</h1>
        <h1 class="shadow">SHOT BY VPD</h1>
        <h1 class="shadow">6-2-20</h1>
      </div>
    </div>
    <div id="agnes_chow" class="relative frame">
      <img src="/agnes.png" />
      <div class="copy">
        <h1 class="shadow">AGNES CHOW</h1>
        <h1 class="shadow">ARRESTED BY CCP</h1>
        <h1 class="shadow">8-10-20</h1>
      </div>
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
    background-image: url('/static.jpg');
}
</style>