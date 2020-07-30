<template>
    <div id="frame">
        <div class="slide flex items-center pl-8">
            <h1 class="now">EVERYTHING IS TEXT</h1>
            <h1 class="subnow magenta">(on the internet)</h1>
        </div>
        <div class="slide">
            <img src="/matrix.png" />
            <h1 class="shadow over now">THIS IS PRETTY ACCURATE</h1>
        </div>
        <div class="slide">
            <img src="/sideby.png" />
        </div>
        <div class="slide">
            <img src="/smith_door.png" />
            <img src="/open_with.png" />
            <img src="/macvim.png" />
            <img src="/image_open.png" />
        </div>
        <div class="slide">
            <img src="/fiji.png" />
        </div>
        <div id="nasir" class="slide">
            <img src="/nasir_jpeg.png" />
        </div>
    </div>
</template>
<style scoped lang="scss">
.slide {
    width: 100vw;
    height: 100vh;
    z-index: 1;
    @apply relative;
}
.over {
    @apply absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    z-index: 2;

}
.shadow {
    color: white;
    text-shadow: 5px 5px 0 #000, -5px -5px 0 #000, -5px 5px 0 #000, 5px -5px 0 #000;
}
#nasir {
    margin-top: 400px;
}
</style>