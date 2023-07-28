<template>
  <div class="">
    <div class="red">
      <div class="banner">
        <picture class="cover">
          <source srcset="../assets/banner.png" media="(min-width: 768px)">
          <img loading="lazy" src="../assets/banner_mobile.png">
        </picture>
      </div>

    </div>
    <div>
      <div class="L-cloud">
        <picture>
          <source srcset="../assets/cloud2.png" media="(min-width: 768px)">
          <img loading="lazy" src="../assets/cloud2_mobile.png">
        </picture>
      </div>
      <div class="R-cloud">
        <picture>
          <source srcset="../assets/cloud.png" media="(min-width: 768px)">
          <img loading="lazy" src="../assets/cloud_mobile.png">
        </picture>
      </div>
    </div>
  </div>
</template>


<style lang="scss" scoped>
@mixin pad {
  @media(min-width:768px) {
    @content;
  }
}

.L-cloud {
  animation: floating-cloud 10s 0.2s linear infinite;
  -webkit-animation: floating-cloud 10s 0.2s linear infinite;
  transform: scale(1.0);
  position: absolute;
  left: 0;
  top: 14rem;

  @include pad {
    top: 22rem;
  }
}

.R-cloud {
  animation: floating-cloud2 10s 0.2s linear infinite;
  -webkit-animation: floating-cloud2 10s 0.2s linear infinite;
  transform: scale(1.0);
  position: absolute;
  right: 0;
  top: 15rem;

  @include pad {
    top: 26rem;
  }
}

@keyframes floating-cloud {
  0% {
    margin-left: 3%;
  }

  50% {
    margin-left: 1%;
  }

  100% {
    margin-left: 3%;
  }

}

@keyframes floating-cloud2 {
  20% {
    margin-right: 4%;
  }

  50% {
    margin-right: 2%;
  }

  100% {
    margin-right: 4%;
  }
}




/* banner */
.banner img {
  width: 100%;
  max-width: 1100px;
  margin: 1rem auto 3rem;
  transform: rotate(-1.118deg);
  position: relative;

  @include pad {
    transform: rotate(0deg);
  }
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
  width: 1.5625rem;
  height: 1.5625rem;
}

.header {
  display: flex;
  justify-content: space-around;
  max-width: 1100px;
  margin: auto;
  background-image: url("../assets/redbg.png");
}
</style>
