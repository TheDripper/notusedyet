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
  padding-left: 20px;
  @apply text-lg mb-6 py-4;
  ul {
    list-style: square;
  }
}
.blink {
  font-size: 60px;
  color: blue;
  @apply mx-auto py-8 w-full;
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
  width: 100vw;
  height: 100vh;
}
.middle {
  @apply flex flex-col items-center justify-center;
}
.shadow {
  color: white;
  text-shadow: 5px 5px 0 #000, -5px -5px 0 #000, -5px 5px 0 #000,
    5px -5px 0 #000;
  box-shadow: none !important;
}
</style>
