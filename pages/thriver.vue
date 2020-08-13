<template>
  <div class="slide flex staticbg">
    <div id="sean_monterrosa" class="relative frame">
      <img src="/thriver_wellness_og.jpg" />
      <img id="thriver_virtual_wellness" :class="{ hidden: hide }" src="/thriver1.jpg" />
      <h1 :class="{ hidden: hide }" class="shadow black">{{ word }}</h1>
    </div>
  </div>
</template>
<style lang="scss" scoped>
#thriver_virtual_wellness {
    filter: saturate(500%) hue-rotate(60deg);
}
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
  img {
    @apply absolute;
    top: 0;
    left: 0;
  }
}
#agnes_chow {
  background: cyan;
  margin-left: 20px;
  .copy {
    margin-top: 20px;
  }
  img {
    @apply absolute;
    top: 0;
    left: 0;
    height: 100%;
    max-width: none;
  }
}
.staticbg {
  background-image: url("/static.jpg");
}
</style>
<script>
export default {
  mounted() {
      let vue = this
    for (let i = 0; i < 1000; i++) {
        
      setTimeout(function () {
          console.log('ding');
          console.log(vue.hide)

          if (vue.hide == true)
            vue.hide = false
          else 
            vue.hide = true
            console.log(vue.word)
          switch (vue.word) {
              case 'VIRTUAL':
                  vue.word = 'WORKPLACE'
                  break;
              case 'WORKPLACE':
                  vue.word = 'WELLNESS'
                  break;
              case 'WELLNESS':
                  vue.word = 'VIRTUAL'
                  break
          }
      }, i * 1000);
    }
  },
  data() {
    return {
      hide: true,
      word: 'WELLNESS',
      black: [
        'VIRTUAL',
      ]
    };
  },
};
</script>