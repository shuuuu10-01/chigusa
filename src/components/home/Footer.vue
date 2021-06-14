<template>
  <section class="footer">
    <img
      src="https://cdn.svgporn.com/logos/youtube-icon.svg"
      @click="toYoutube"
    />
    <img
      src="https://cdn.svgporn.com/logos/twitter.svg"
      @click="toTwitter"
    />
    <div>2021 © shuuuu</div>
  </section>
</template>

<script>
export default {
  methods: {
    toYoutube () {
      open('https://t.co/3lrTPKCQIW?amp=1')
    },
    toTwitter () {
      open('https://twitter.com/Chigusa_24zono')
    }
  }
}
</script>

<style scoped>
.footer {
  margin: auto;
}
img {
  width: 30px;
  margin-left: 20px;
  margin-right: 20px;
  margin-bottom: 10px;
  cursor: pointer;
}
img:hover {
  opacity: 0.5;
}
</style>
