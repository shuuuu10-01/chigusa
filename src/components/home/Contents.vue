<template>
  <section>
    <div class="wrap">
      <p class="bg"><img src="../../assets/ideltalk.jpeg" alt="ideltalk"></p>
      <title-and-description
        class="txt"
        title="IDEL TALK"
        description="たくさんコメントを読んでくれる。推しの話になると暴走列車。落ち着く声で気付いたら時間が溶けてる。君も沼にハマらないか？"
      />
    </div>
    <div class="wrap" id="sec02_02">
      <p class="bg"><img src="../../assets/song.jpeg" alt="song"></p>
      <title-and-description
        class="txt"
        title="SONG"
        description="綺麗な歌声でいつも癒される。時間帯に合わせて選曲してくれる。深夜の歌配信ではいつの間にか夢の中へ。。。"
      />
    </div>
    <div class="wrap">
      <p class="bg"><img src="../../assets/game.jpeg" alt="game"></p>
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
}

img{
  width: 100%;
  height: auto;
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
  }
}
</style>
