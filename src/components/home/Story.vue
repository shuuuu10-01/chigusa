<template>
  <div class="story">
    <title-and-description
      title="Story"
      description="創立から優に100年を超える、由緒ある学校「世怜音女学院（せれいねじょがくいん）」。
      「文武両道」を掲げ、生徒はもれなく部活動に勤しむことを義務付けられている。
      そんな学院において、かつては栄華を誇った部活動がひとつ。
      今は部員も足りず、同好会にまで格下げされてしまった「元演劇部」。
      そこへ加わる新入生と、それから転校生。
      ふたりを迎えた「学院演劇同好会」は、今新たな門出を迎える。
      5人が目指すは「部への昇格」と、「学院祭での演目の実施」。
      果たして、5人の悲願は叶うのか。"
    />
  </div>
</template>

<script>
import TitleAndDescription from './TitleAndDescription.vue'
export default {
  components: { TitleAndDescription }

}
</script>

<style scoped>
.story {
  background: url('https://pbs.twimg.com/profile_banners/1289884632637349888/1613001450/1080x360') no-repeat 100% 100% fixed;
  background-position: center;
  background-size: cover;
  -webkit-background-size: cover;
  color: #fff;
  padding-bottom: 80px;
}
</style>
