<template>
  <section>
    <div class="wrap">
      <p class="bg"><img src="https://pbs.twimg.com/media/E0XrUsGVkAMrylG?format=jpg&name=large" alt="ideltalk"></p>
      <title-and-description
        class="txt"
        title="IDEL TALK"
        description="たくさんコメントを読んでくれる。推しの話になると暴走列車。落ち着く声で気付いたら時間が溶けてる。君も沼へはまってみませんか？"
      />
    </div>
    <div class="wrap" id="sec02_02">
      <p class="bg"><img src="https://pbs.twimg.com/media/EmoZi9sWEAgiVR3?format=jpg&name=large" alt="song"></p>
      <title-and-description
        class="txt"
        title="SONG"
        description="透き通ってて綺麗な歌声でいつも癒される。時間帯に合わせて選曲してくれる。深夜の歌配信ではいつの間にか夢の中へ。。。"
      />
    </div>
    <div class="wrap">
      <p class="bg"><img src="https://pbs.twimg.com/media/EwGBosPUYAIgz5U?format=jpg&name=large" alt="game"></p>
      <title-and-description
        class="txt"
        title="GAME"
        description="日に日に上手くなっていくAPEX。推しに全力投球なウマ娘。バイオハザードはギャルゲー。あなほりポケモンには要注意、ショタトレーナーは逃げて！！"
      />
    </div>
  </section>
</template>

<script>
import TitleAndDescription from '../home/TitleAndDescription.vue'
export default {
  components: {
    TitleAndDescription
  }
}
</script>

<style scoped>
.wrap{
  clear: both;
  width: 100%;
  background: #f6f6f6;
}

img{
  width: 100%;
  height: auto;
}
section .txt{
  padding-bottom: 80px;
}

@media only screen and (min-width: 800px){
  .txt, .bg{
    width: 50%;
    float: left;
    display: table;
    margin-top: 40px;
  }

  #sec02_02 .txt, #sec02_02 .bg{
    float: right;
  }

  .txt {
    background: #f6f6f6;
    display: table-cell;
  }
}
</style>
