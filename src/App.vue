<template>
  <HeaderNav />
  <SectionBanner />
  <SectionGame />
  <SectionMap />
  <SectionQA />
  <SectionContent />
  <SectionFooter />
</template>

<script>
import HeaderNav from './components/HeaderNav.vue'
import SectionBanner from './components/SectionBanner.vue'
import SectionGame from './components/SectionMap.vue'
import SectionMap from './components/SectionGame.vue'
import SectionQA from './components/SectionQA.vue'
import SectionContent from './components/SectionContent.vue'
import SectionFooter from './components/SectionFooter.vue'
export default {
  name: 'App',
  components: {
    HeaderNav,
    SectionBanner,
    SectionMap,
    SectionGame,
    SectionQA,
    SectionContent,
    SectionFooter
  }
}
</script>

<style>
:root {
  --main-black-color: #2B2828;
  --main-yellow-color: #D6BC5C;
  --main-red-color: #CF3319;
  font-family: 'Noto Sans TC', sans-serif;
  --content-fontsize: 1.2rem;
  --title-fontsize: 1.875rem;
  ;

}

html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
}

/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
  display: block;
}

body {
  line-height: 1;
}

ol,
ul {
  list-style: none;
}

blockquote,
q {
  quotes: none;
}

blockquote:before,
blockquote:after,
q:before,
q:after {
  content: '';
  content: none;
}

table {
  border-collapse: collapse;
  border-spacing: 0;
}

#app {
  text-align: center;
  background-image: url('./assets/bg.png');
  height: 100vh;
  margin: auto;
}

body {
  background-image: url('./assets/bg.png');
  height: 100vh;
}



h2 {
  color: var(--main-black-color);
  text-align: justify;
  font-family: Noto Serif TC;
  font-size: var(--title-fontsize);
  font-weight: 600;
  line-height: normal;
  letter-spacing: 0.09375rem;
  text-align: center;
}

h3 {
  color: #F1F3F4;
  font-family: Noto Serif TC;
  font-size: var(--title-fontsize);
  font-style: normal;
  font-weight: 700;
  line-height: normal;
  letter-spacing: 0.09375rem;
}

.layout {
  max-width: 1400px;
  margin: auto;
  width: 100%;
}

.red {
  background-image: url("./assets/redbg.png");
}
</style>
