<template>
  <div class="">
    <div class="red">
      <div class="header">
        <div class="logo">
          <a><img src="../assets/logo.png" alt=""></a>
        </div>
        <div class="container navbar">
          <a>廟宇介紹</a>
          <a>神機廟算</a>
          <a>奇思廟想</a>
          <a>廟語如珠</a>
          <a>錦囊妙劇</a>
        </div>
        <div class="share">
          <a><img src="../assets/fb.png" alt=""></a>
          <a><img src="../assets/line.png" alt=""></a>
          <a><img src="../assets/link.png" alt=""></a>
        </div>
      </div>
    </div>
  </div>
</template>



<style scoped>
.share {
  display: flex;
  justify-content: space-around;
  gap: 1rem;
}

.red {
  background-image: url("../assets/redbg.png");
}

/* header */
.header div {
  display: flex;
  align-items: center;
}

.header>.share img {
  width: 2rem;
  height: 2rem;
}

.header {
  display: flex;
  justify-content: space-around;
  max-width: 1400px;
  margin: auto;
  background-image: url("../assets/redbg.png");
}


.container a {
  color: #F1F3F4;
  position: relative;
  cursor: pointer;
  margin: .5rem 1rem;
  font-family: 'Noto Serif TC', serif;
  font-size: 1.5rem;
  padding: .5rem;
}

.navbar a:after {
  position: absolute;
  opacity: 0;
  width: 0%;
  height: 2px;
  left: 0px;
  content: '';
  background: #FFF;
  transition: all 0.3s;
  bottom: 0px;
}

.navbar a:hover:after {
  opacity: .8;
  width: 100%;
}

.logo {

  display: flex;
}

.logo img {
  width: 250px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 2rem auto;
}
</style>
