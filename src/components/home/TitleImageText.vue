<template>
  <div class="col3">
    <h2>{{ title }} </h2>
    <img :src="image" alt=""/>
    <p>{{ text }}</p>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    image: {
      type: String,
      required: true
    },
    text: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
img {
  max-width: 288px;
  width: 100%;
  display: block;
  margin: -5px auto 20px;
  border: 2px;
  border-radius: 50%;
  border-color: black;
}
.col3 {
  text-align: center;
  margin: auto;
}
h2 {
  font-size: 18px;
  margin: auto;
  font-family: 'Noto Sans JP';
}
p {
  font-family: 'Noto Sans JP';
}
</style>
