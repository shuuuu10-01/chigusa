<template>
  <div class="header">
    <img src="../../assets/headerImage.png" />
    <div class="slogan">
      <h1>Chihgusa Nishizono</h1>
      <h2>#にじさんじ #セレ女 #舞元の元嫁</h2>
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
  height: 600px;
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
  text-shadow: 2px 1px 3px rgba(0,0,0,0.3);
}

.slogan h2 {
  font-size: 20px;
  font-family: 'Noto Sans JP';
  font-weight:normal;
  text-shadow: 2px 1px 3px rgba(0,0,0,0.3);
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
