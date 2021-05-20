<template>
  <section>
    <h2>
      Latest Videos
    </h2>
    <div class="videos" v-for="i in videoList" :key="i.num">
      <thumbnail :thumbnail="i.thumbnail" :title="i.title" :description="i.description" :id="i.id"/>
    </div>
  </section>
</template>

<script>
import Thumbnail from './Thumbnail.vue'
export default {
  components: { Thumbnail },
  data () {
    return {
      videoList: []
    }
  },
  async created () {
    const params = {
      part: 'snippet',
      channelId: 'UCkngxfPbmGyGl_RIq4FA3MQ',
      type: 'video',
      maxResults: 3,
      order: 'date',
      key: String(process.env.VUE_APP_YOUTUBE_API_KEY)
    }
    this.axios
      .get('https://www.googleapis.com/youtube/v3/search', {
        params: params
      })
      .then((result) => {
        this.videoList = result.data.items.map((item) => ({
          id: item.id.videoId,
          title: item.snippet.title,
          description: item.snippet.description,
          thumbnail: item.snippet.thumbnails.medium.url
        }))
        this.videoList.reverse()
      })
  }
}
</script>

<style scoped>
section {
  display: inline-block;
  padding-bottom: 40px;
  width: 100%;
}
</style>
