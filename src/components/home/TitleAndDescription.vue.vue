<template>
  <section>
    <header>
      <h2>{{ title }}</h2>
    </header>
    <div class="character">
      {{ description }}
    </div>
  </section>
</template>

<script>
export default {
  props: {
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
.character{
  width: 60%;
  margin: 0 auto;
  padding-bottom: 80px;
  font-size: 14px;
  font-family: 'Noto Sans JP';
}
</style>
