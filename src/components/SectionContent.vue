<template>
  <div>
    <div class="red" id="article">
      <div class="layout c">
        <h3>廟語如珠</h3>
        <div class="content" v-for="item in member" :key="item.id">
          <a class="content_tag" :src="'https://www.ftvnews.com.tw/news/detail/' + id">
            {{ item }}
          </a>
          <a class="content_text">授權文章授權文章授權文章授權文章授權文章授權文章授權文章授權文章授權文章文章授權文章文章
          </a>
        </div>
        <div class="news" v-for="(item, index) in news" :key="index">

          <div>
            <a :href="'https://www.ftvnews.com.tw/news/detail/' + item.ID" target="_blank">{{ item.Title }}</a>
          </div>
        </div>
      </div>

    </div>
    <div class="layout" id="video">
      <h3>錦囊妙劇</h3>
      <div class="video_layout">
        <a href="http://" target="_blank" v-for="item in video" :key="item.id" rel="noopener noreferrer">
          <img loading="lazy" class="video" src="../assets/video.png" alt="">
          相關影音相關影音相關影音相關影音相關影音相關影音相關影音相關影音</a>
      </div>
    </div>
  </div>
</template>
,台灣廟世界
<script>
export default {
  data() {
    return {
      member: ['廟宇介紹', '籤詩解釋', '奇廟世界', '籤詩解釋', '奇廟世界', '廟宇介紹', '籤詩解釋', '奇廟世界', '籤詩解釋', '奇廟世界'],
      video: ['廟宇介紹', '籤詩解釋', '奇廟世界']
    }
  },
}
</script>

<style lang="scss" scoped>
@mixin pad {
  @media(min-width:768px) {
    @content;
  }
}

h3 {
  text-align: start;
  padding: 1.5rem 0rem;
  border-bottom: 2px solid white;
}

.c {
  width: 100%;
}

.video_layout {
  display: flex;
  flex-direction: row;
  gap: 2rem;
  margin-top: 2rem;
  width: 100%;
  overflow-x: scroll;

  a {
    text-align: start;
    color: #FFF;
    text-align: justify;
    font-size: var(--content-fontsize);
    font-weight: 500;
    line-height: normal;
    letter-spacing: 0.0625rem;
    text-decoration: none;
    border-bottom: 2px dashed white;
  }

  .video {
    height: 13rem;
    border-radius: 0.625rem;
    background: #D9D9D9;
    box-shadow: 0px 4px 4px 0px #974213;
  }

}



.red {
  margin-top: -2px;
  padding: 1rem;
  display: flex;
  flex-direction: column;
  gap: 2rem;
  background-image: url("../assets/redbg.png");
}



.layout a {
  padding: 1.5rem 0rem;
  font-size: var(--content-fontsize);
  color: #F1F3F4;
}

.content_tag {
  text-align: start;
  border-bottom: 2px dashed white;
}

.content_text {
  text-align: end;
  border-bottom: 2px dashed white;
}

.content {
  width: 100%;
  display: grid;
  grid-template-columns: 1fr 9fr;
}

.all {
  text-align: end;
  width: 100%;
}
</style>
