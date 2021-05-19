<template>
  <div class="header">
    <img src="https://pbs.twimg.com/media/Etes-qOVEAArYDY?format=png&name=large" />
    <div class="slogan">
      <h1>Chihgusa Nishizono</h1>
      <h2>#にじさんじ #セレ女 #舞元の姪</h2>
    </div>
  </div>
</template>

<script>
export default {
}
</script>

<style scoped>
.header {
  position: relative;
  overflow: hidden;
  width: 100%;
  height: 700px;
}
img {
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  width: 1000px;
}
.slogan {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: #b6c9f0;
  width: 80%;
}
.slogan h1{
  font-size: 50px;
  font-family: 'Pacifico', cursive;
  margin-bottom: 20px;
  font-weight:normal;
  text-shadow: var(--slogan-shadow);
}

.slogan h2 {
  font-size: 20px;
  font-family: 'Noto Sans JP';
  text-shadow: var(--slogan-shadow);
}

@media only screen and (max-width: 599px){
  .slogan h1{
    font-size: 36px;
  }

  .slogan h2{
    font-size: 16px;
  }
}
</style>
