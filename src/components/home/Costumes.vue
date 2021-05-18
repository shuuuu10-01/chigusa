<template>
  <section>
    <h2>COSTUME</h2>
    <ul class="col3">
      <li>
        <title-image-text
          title="初期衣装"
          :image="getImage('first.png')"
          text="きれいな青のショートカット。笑ったときの八重歯に一目惚れ。
          制服のジャケットの下にパーカーとシャツを着ている。多分ごわつく。"
        />
      </li>
      <li>
        <title-image-text
          title="新衣装"
          :image="getImage('new.png')"
          text="待ちに待った新衣装。長髪メガネ帽子チョーカー網タイツ女子に進化。緩いパーカーがどストレート。
          個人的にはショート帽子チョーカー網タイツが好み。"
        />
      </li>
      <li>
        <title-image-text
          title="にゃんめんぎょ"
          image="https://pbs.twimg.com/media/EfMXrnYU8AEdboq?format=jpg&name=900x900"
          text="初期衣装ではパーカーにプリントされており、新衣装ではバッグのキーホルダーで登場している。将来世界中を癒すであろう超絶大型新人ゆるキャラ"
        />
      </li>
    </ul>
  </section>
</template>

<script>
import TitleImageText from './TitleImageText.vue'
export default {
  components: { TitleImageText },
  methods: {
    getImage (filename) {
      return require('../../assets/' + filename)
    }
  }
}
</script>

<style scoped>
section {
  display: inline-block;
  width: 90%;
  max-width: 1100px;
  padding-bottom: 80px;
}
.top {
  margin-top: 20px;
  width: 100%;
}
.col3 li{
  margin-bottom: 50px;
}

@media only screen and (min-width: 800px){
  .col3 {
    text-align: center;
  }

  .col3 li{
    display: inline-block;
    width: 30%;
    padding: 0 1.5%;
    margin-bottom: 0;
    vertical-align: top;
    text-align: left;
  }
}

@media only screen and (max-width: 799px){
  .col3 li {
    margin: 0 auto;
    display: block;
    max-width: 288px;
  }
}
</style>
