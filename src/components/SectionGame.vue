<template>
  <div class="layout_game">
    <div class="game_content">
      <p>神機妙算</p>
      <p> 我們現在在OOOO的正殿這尊月神明是OOOO。
        請帶著虔誠的心，向神明自我介紹，結束後，請告訴月老你最近在煩惱什麼...？</p>
    </div>
    <div class="img_paper">
      <a data-tf-popup="HfrtIHhy" data-tf-opacity="100" data-tf-size="70"
        data-tf-iframe-props="title=Picture quiz template (copy)" data-tf-auto-close="1000"
        data-tf-transitive-search-params data-tf-medium="snippet" style="cursor:pointer;">
        <div class="btn_game" alt=""></div>
      </a>
    </div>

  </div>
</template>
<style scoped>
.game_content {
  color: var(--unnamed, #2B2828);
  font-family: Noto Serif TC;
  font-size: 1.375rem;
  font-weight: 600;
  line-height: normal;
  text-align: start;
  margin: auto;
  position: relative;
}

.game_content p {
  font-size: var(--title-fontsize);
}

.layout_game {
  background-image: url('../assets/gamebg2.png');
  width: 100%;
  height: 100%;
  max-height: 26rem;
  max-width: 1300px;
  margin: auto;
  background-position-x: center;
  background-size: contain;
  background-repeat: no-repeat;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.btn_game {
  content: url('../assets/1.png');
  width: 100%;
  margin: auto;
  display: flex;
  justify-content: center;
}

.btn_game:hover {
  content: url('../assets/2.png');
  transform: .2s all;
  cursor: pointer;
}

.img_paper {
  position: relative;
}

@media screen and (min-width: 768px) {
  .btn_game {
    content: url('../assets/1.png');
  }

  .btn_game:hover {
    content: url('../assets/2.png');
  }
}

.img_paper:hover {
  filter: drop-shadow(2px 4px 4px rgba(0, 0, 0, 0.1));
  transition: .2s all;
}
</style>
