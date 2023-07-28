<template>
  <div>
    <div class="red">
      <div class="header">
        <div class="logo">
          <a><img src="../assets/logo.png" alt=""></a>
        </div>
        <div class="computer">
          <div class="container navbar">
            <a href="#intro">廟宇介紹</a>
            <a href="#game">神機廟算</a>
            <a href="#qa">奇思廟想</a>
            <a href="#article">廟語如珠</a>
            <a href="#video">錦囊妙劇</a>
          </div>
          <div class="share">
            <a><img src="../assets/fb.png" alt=""></a>
            <a><img src="../assets/line.png" alt=""></a>
            <a><img src="../assets/link.png" alt=""></a>
          </div>
        </div>

      </div>
      <div>
        <div class="mobile_nav">
          <div class="logo">
            <a><img src="../assets/logo.png"></a>
          </div>
          <h3 class="bars" @click="toggleMobileMenu"><img src="../assets/bars.png" alt=""></h3>
        </div>
        <div class="mobile_menu" :style="{ display: isMobileMenuVisible ? 'flex' : 'none' }" alt="">
          <a>廟宇介紹</a>
          <a>神機廟算</a>
          <a>奇思廟想</a>
          <a>廟語如珠</a>
          <a>錦囊妙劇</a>
          <div class="mobile_share">
            <a><img src="../assets/fb.png" alt=""></a>
            <a><img src="../assets/line.png" alt=""></a>
            <a><img src="../assets/link.png" alt=""></a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isMobileMenuVisible: false,
    };
  },
  methods: {
    toggleMobileMenu() {
      this.isMobileMenuVisible = !this.isMobileMenuVisible;
    },
  },
};
</script>

<style lang="scss" scoped>
.red {
  background-image: url("../assets/redbg.png");
}

.share {
  display: flex;
  justify-content: space-around;
  gap: 1rem;

  img {
    width: 2rem;
    height: 2rem;
  }
}

.header {
  display: flex;
  justify-content: space-around;
  max-width: 1100px;
  margin: auto;
  background-image: url("../assets/redbg.png");

  div {
    display: flex;
    align-items: center;
  }
}

.logo {
  display: flex;

  img {
    width: 250px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 2rem auto;
  }
}

.container {
  a {
    color: #F1F3F4;
    position: relative;
    cursor: pointer;
    margin: .5rem 1rem;
    font-family: 'Noto Serif TC', serif;
    font-size: 1.5rem;
    padding: .5rem;
  }
}

.navbar {
  a {
    &:after {
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

    &:hover:after {
      opacity: .8;
      width: 100%;
    }
  }
}

.bars {
  display: flex;
  justify-content: center;
  padding: 1rem auto;
  width: fit-content;
  position: fixed;
  top: 1rem;
  right: 1rem;
  animation: none;
  background-image: url("../assets/redbg.png");
  background-size: 20%;
  background-size: small;
  box-shadow: rgba(0, 0, 0, 0.4) 0px 2px 4px, rgba(0, 0, 0, 0.3) 0px 7px 13px -3px, rgba(0, 0, 0, 0.2) 0px -3px 0px inset;
}



.mobile_menu {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  width: -moz-fit-content;
  width: fit-content;
  padding: 1rem;
  position: fixed;
  top: 3rem;
  right: 1rem;
  z-index: 9999999;
  background-image: url("../assets/redbg.png");

  a {
    color: #F1F3F4;
    font-family: Noto Serif TC;
    font-size: 18px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
    border-bottom: 1px solid #F1F3F4;
  }
}

.mobile_nav {
  display: flex;
  justify-content: space-between;
  background-image: url("../assets/redbg.png");
  width: 80%;
  align-items: center;


  .logo img {
    width: 180px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 1rem auto;
  }
}

.mobile_share img {
  width: 30px
}



.header {
  display: none;
}

@media screen and (min-width:768px) {

  .header {
    display: flex;
  }

  .mobile_nav {
    display: none;
  }

}
</style>
