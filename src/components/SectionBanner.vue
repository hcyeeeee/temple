<template>
  <div class="">
    <div class="red">
      <div class="banner">
        <img src="../assets/banner.png" class="cover" alt="">
      </div>
    </div>
    <div>
      <div class="L-cloud">
        <img src="../assets/cloud2.png" alt="">
      </div>
      <div class="R-cloud">
        <img src="../assets/cloud.png" alt="">
      </div>
    </div>
  </div>
</template>



<style scoped>
.L-cloud {
  animation: floating-cloud 10s 0.2s linear infinite;
  -webkit-animation: floating-cloud 10s 0.2s linear infinite;
  transform: scale(1.0);
  position: absolute;
  left: 0;
  top: 20rem
}

.R-cloud {
  animation: floating-cloud2 10s 0.2s linear infinite;
  -webkit-animation: floating-cloud2 10s 0.2s linear infinite;
  transform: scale(1.0);
  position: absolute;
  right: 0;
  top: 25rem
}

@keyframes floating-cloud {
  0% {
    margin-left: 1%;
  }

  50% {
    margin-left: -3%;
  }

  100% {
    margin-left: 1%;
  }
}

@keyframes floating-cloud2 {
  20% {
    margin-right: -2%;
  }

  50% {
    margin-right: 1%;
  }

  100% {
    margin-right: -2%;
  }
}


/* banner */
.banner img {
  width: 100%;
  max-width: 1200px;
  margin: 1rem auto 3rem;
  transform: rotate(-1.118deg);
  position: relative;
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
  max-width: 1300px;
  margin: auto;
  background-image: url("../assets/redbg.png");
}
</style>
