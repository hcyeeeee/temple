<template>
  <div class="layout_game" id="game">
    <div class="game_content">
      <h3>神機妙算</h3>
      <p> 我們在中壢仁海宮的正殿<br>
        這尊神明是天上聖母。<br>
        請帶著虔誠的心，<br>
        向天上聖母自我介紹，<br>
        結束後，請告訴天上聖母<br>
        你最近在煩惱什麼．．．？</p>
      <a data-tf-popup="M5UMm1mf" data-tf-opacity="100" data-tf-hide-headers data-tf-size="80"
        data-tf-iframe-props="title=廟宇求籤" data-tf-auto-close="0" data-tf-transitive-search-params data-tf-medium="snippet"
        style="cursor:pointer;">
        <div class="btn_game" alt=""></div>
      </a>
    </div>
    <div class="thanks_layout">
      <h3 class="thanks_title">
        特別感謝 - 仁海宮 支援詩籤
      </h3>
      <div class="thanks_content">
        仁海宮是一座有兩百年歷史悠久的廟宇，立於市區，處於南北要道，外觀氣勢雄偉，屋頂飛簷，樓宇雕樑畫棟，五彩繽紛，極具傳統廟宇建築風格，親近它，會發思幽懷古之情，經多次增建整建後，巍峨壯麗，場地寬暢，每座神龕金碧輝煌尊隆神聖,各項祭祀活動，善男信女，十方大德眾多人潮參與，仁海宮香火更為興盛。
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

.layout_game {
  font-family: Noto Serif TC;
  display: grid;
  grid-template-columns: 1fr;
  width: 90%;
  margin: 1rem auto;
  padding: -2rem;
  place-content: center;
  gap: 2rem;

  @include pad {
    max-width: 1100px;
    width: 100%;
    grid-template-columns: 1fr 1fr;
    margin: 3rem auto;
  }

  .thanks_layout {
    .thanks_title {
      border-radius: 1.25rem 1.25rem 0rem 0rem;
      background: var(--unnamed, #CF3319);
      padding: 1rem;
      color: #F1F3F4;
      font-size: var(--content-fontsize);
      text-align: center;
    }

    .thanks_content {
      font-size: 1.2rem;
      border-radius: 1.25rem;
      display: flex;
      padding: 1.5rem;
      height: 230px;
      box-shadow: 1px 2px 4px 0px rgba(0, 0, 0, 0.25);
      background-image: url('../assets/templebg.png');
      line-height: 150%;
      text-align: start;

    }
  }
}

.game_content {
  color: var(--main-black-color);
  font-size: var(--content-fontsize);
  display: flex;
  padding: 1rem;
  padding: 2.4rem 1rem;
  gap: 1rem;
  justify-content: space-evenly;
  align-items: center;
  background-image: url('../assets/gamebg.png');
  background-size: cover;
  box-shadow: 1px 2px 4px 0px rgba(0, 0, 0, 0.25);

  @include pad {
    gap: 3rem;
    padding: 2rem;
  }

  .btn_game {
    content: url('../assets/茭.png');
    width: 100%;
    margin: auto;
    width: 6rem;

    &:hover {
      content: url('../assets/茭2.png');
      transform: .2s all;
      cursor: pointer;
    }
  }

  h3 {
    font-size: var(--title-fontsize);
    background: #CF3319;
    width: fit-content;
    box-shadow: 2px 2px 2px 0px rgba(0, 0, 0, 0.10);
    -webkit-writing-mode: vertical-lr;
    writing-mode: vertical-lr;
    position: relative;
    padding: 0.5rem;
    top: -6rem;
    font-weight: 600;
    letter-spacing: .4rem;
    box-shadow: 2px 2px 2px 0px rgba(0, 0, 0, 0.10);
  }

  p {
    font-size: 1.2rem;
    color: var(--unnamed, #2B2828);
    -webkit-writing-mode: vertical-lr;
    writing-mode: vertical-lr;
    text-align: start;
    line-height: 130%;
    gap: 1rem;
    letter-spacing: .2rem;

    @include pad {
      line-height: 150%;
    }
  }


}
</style>
