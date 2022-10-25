<template>
  <router-view/>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;600&display=swap');
/* font-family: 'Outfit', sans-serif; */

*, *::before, *::after {
  box-sizing: border-box;
}
* {
  margin: 0;
}
html, body {
  height: 100%;
}
body {
  line-height: 1.5;
  -webkit-font-smoothing: antialiased;
}
img, picture, video, canvas, svg {
  display: block;
  max-width: 100%;
}
input, button, textarea, select {
  font: inherit;
}
p, h1, h2, h3, h4, h5, h6 {
  overflow-wrap: break-word;
}
#root, #__next {
  isolation: isolate;
}

body{
  font-size: 18px;
}
:root{
  /* primary */
  --softblue: hsl(215, 51%, 70%);
  --cyan: hsl(178, 100%, 50%);
  
  /* neutral */
  --main-bg: hsl(217, 54%, 11%);
  --card-bg: hsl(216, 50%, 16%);
  --line: hsl(215, 32%, 27%);
  --white: hsl(0, 0%, 100%);
}
</style>
