<template>
  <div class="video">
    <img :src="thumbnail" />
    <div class="text">
      <h2>{{ title }}</h2>
      <p>{{ description }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    thumbnail: {
      type: String,
      required: true
    },
    title: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
.video {
  display: flex;
  width: 90%;
  max-width: 1100px;
  margin: auto;
  margin-bottom: 15px;
  padding: 10px;
  box-shadow: var(--video-shadow);
  overflow: hidden;
  cursor: pointer;
}
.video:hover{
  box-shadow: var(--hover-shadow);

}
.text {
  margin-left: 10px;
  text-align: left;
}
.text h2, p {
  display: -webkit-box;
  -webkit-line-clamp: 2;
  text-overflow: ellipsis;
  white-space: normal;
  overflow: hidden;
  -webkit-box-orient: vertical;
  padding: 0;
  font-family: 'Josefin Sans', 'Noto Sans JP',serif;;
}

.text h2 {
  text-align: left;
  font-size: 22px;
  padding-top: 2px;
}
img {
  max-width: 300px;
}

@media only screen and (max-width: 640px){
  .text h2 {
    font-size: 15px;
  }
  img {
    width: 50%;
  }
  .text {
    width: 50%;
  }
}
</style>
