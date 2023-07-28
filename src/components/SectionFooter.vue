<template>
  <div class="footer_layout">
    <p>文字內容｜郭家妤、廖婉馨、徐薇淳 &nbsp;&nbsp;視覺設計｜周映璇&nbsp;&nbsp; 網頁設計｜黃莘懿
      <br>Copyright © 2023 民視新聞網路部 社群中心
    </p>

  </div>
</template>


<style lang="scss" scoped>
@mixin pad {
  @media(min-width:768px) {
    @content;
  }
}

.swiper {
  width: 100%;
  height: 600px;
}

.footer_layout {
  font-size: 1rem;
  font-weight: 500;
  line-height: 2rem;
  font-family: Noto Serif TC;
  background-image: url('../assets/footer.png');
  width: 100%;
  background-color: #cd3118;
  background-size: cover;
  padding-top: 1rem;

  @include pad {
    font-size: var(--content-fontsize);
  }
}

p {
  margin: auto;
  margin-top: 1rem;
  margin: 2rem;
  padding-top: 2rem;
  padding-bottom: 2rem;

}
</style>
