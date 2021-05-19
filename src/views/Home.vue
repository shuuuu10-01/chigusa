<template>
  <div class="home">
    <title-and-description style="padding-bottom: 80px;" :title="title" :description="description"/>
    <contents />
    <costumes />
    <story />
    <latest-video />
  </div>
</template>

<script>
import Contents from '../components/home/Contents.vue'
import Costumes from '../components/home/Costumes.vue'
import LatestVideo from '../components/home/LatestVideo.vue'
import Story from '../components/home/Story.vue'
import TitleAndDescription from '../components/home/TitleAndDescription.vue'

export default {
  name: 'Home',
  components: {
    TitleAndDescription,
    Contents,
    Costumes,
    Story,
    LatestVideo
  },
  data () {
    return {
      title: 'CHARACTER',
      description: '世怜音女学院（通称セレ女）の高等部に通う2年生。太もものほくろと元気いっぱいの笑顔がトレンドマークの女の子。BLとゲームが大好き。某馬アプリに14万課金したとこで「14万の女」とよばれることもしばしば。推しに対して財布の紐が緩く、視聴者からも共感されている。ホラーゲームの敵キャラを恋愛ゲームの攻略対象と思い込むことで怖さを克服しようとした。また、韓国語を話すことができ、APEXの大会では韓国の有名なプロゲーマーと共闘し、熱い試合を繰り広げた。ショタコン。'
    }
  }
}
</script>
