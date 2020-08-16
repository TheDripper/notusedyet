<template>
  <div>
    <nuxt />
  </div>
</template>

<style lang="scss">
.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
html,
body {
  background: cyan;
  font-family: "vcr";
}
@font-face {
  font-family: "vcr";
  src: url("/vcr.ttf");
}
p {
  @apply mb-6 text-lg;
}
ul {
  list-style: circle;
  padding-left: 40px;
  @apply text-lg mb-6 py-4;
  ul {
    list-style: square;
  }
}
.blink {
  font-size: 60px;
  animation: blink-animation 2s steps(5, start) infinite;
  -webkit-animation: blink-animation 2s steps(5, start) infinite;
}
.scroll {
  animation: scroll 5s steps(5, start) infinite;
}
@keyframes scroll {
  to {
    margin-left: -700px;
  }
}
@keyframes blink-animation {
  to {
    visibility: hidden;
  }
}
@-webkit-keyframes blink-animation {
  to {
    visibility: hidden;
  }
}
li {
  @apply mb-4 text-lg;
}

ol {
  list-style: decimal;
  @apply pl-12;
}
a {
  text-decoration: underline;
  color: blue;
  @apply p-2;
  border: 2px solid #00ff00;
}
.container {
  max-width: 100%;
}
iframe {
  max-width: 100%;
}
.now {
  font-size: 60px;
}
.magenta {
  color: magenta;
}
.subnow {
  font-size: 30px;
}
.slide {
  width: calc(100vw - 3rem);
  height: 100vh;
}
.middle {
  @apply flex flex-col items-center justify-center;
}

.shadow {
  color: white;
  text-shadow: 3px 3px 0 #000, -3px -3px 0 #000, -3px 3px 0 #000,
      3px -3px 0 #000;
  @screen md {
    text-shadow: 5px 5px 0 #000, -5px -5px 0 #000, -5px 5px 0 #000,
      5px -5px 0 #000;
  }
  box-shadow: none !important;
  
}
.black {
    color: black !important;
    text-shadow: 5px 5px 0 lime, -5px -5px 0 lime, -5px 5px 0 lime,
      5px -5px 0 lime;
  }
li {
  font-size: 30px;
  list-style: none;
  position: relative;
  padding-left: 34px;
  a {
    border: 5px solid blue !important;
  }
  &:before {
    content: "#!";
    color: magenta;
    position: absolute;
    left: -34px;
    top: 0;
    animation: blink-animation 2s steps(5, start) infinite;
    transform: scale(1.7);
  }
}
.text-white {
  color: white !important;
}
#until {
  font-size: 80px !important;
}
#actual_patriarchy {
  a {
    color: white !important;
  }
}
#occupy_venture_capital_until {
  a {
    color: white !important;
  }
}
@keyframes blink-animation {
  to {
    visibility: hidden;
  }
}
.off {
  animation: off 1s;
  animation-fill-mode: forwards;
}
@keyframes off {
  to {
    opacity: 0;
  }
}
.sat {
  animation: sat 1s;
  animation-fill-mode: forwards;
}
@keyframes sat {
  to {
    filter: saturate(500) hue-rotate(90deg);
  }
}
@keyframes fade {
  to {
    opacity: 0;
    margin-bottom: -50px;
  }
}
.fade {
  animation: fade 1s;
  animation-fill-mode: forwards;
}
@keyframes slide {
  to {
    margin-left: -3000px;
  }
}
@keyframes slide-right {
  to {
    margin-left: 3000px;
  }
}
.slide-off {
  animation: slide 20s;
  animation-fill-mode: forwards;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}
.slide-right {
  animation: slide-right 20s;
  animation-fill-mode: forwards;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}
@keyframes zoom {
  to {
    transform: scale(20) rotate(50deg);
    filter: saturate(500%) hue-rotate(280deg) contrast(200%);
    opacity: 0.3;
  }
}
.zoom {
  animation: zoom 1s;
  animation-fill-mode: forwards;
}
.colors_fast {
  animation: colors 5s;
}
.colors_fast {
  animation: colors 1s infinite;
}
@keyframes colors {
  0% {
    color: magenta;
  }
  20% {
    color: lime;
  }
  40% {
    color: cyan;
  }
  60% {
    color: red;
  }
  80% {
    color: purple;
  }
  
}
.scroll_frame {
  position: relative;
  overflow: hidden;
}
</style>
