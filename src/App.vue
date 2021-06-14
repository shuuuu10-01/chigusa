<template>
  <div id="app">
    <Header />
    <router-view/>
    <Footer />
  </div>
</template>

<script>
import Footer from './components/home/Footer.vue'
import Header from './components/home/Header.vue'
export default {
  components: { Header, Footer }
}
</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Pacifico);
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+JP');
@import url(https://fonts.googleapis.com/css?family=Josefin+Sans);

:root {
  --slogan-shadow: 2px 2px 3px rgba(255, 60, 60, 0.3);
  --video-shadow:  0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
  --hover-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
  --rounded: 0.25rem;
}

/* reset */
body,div,dl,dt,dd,ul,ol,li,h1,h2,h3,h4,h5,h6,pre,form,fieldset,input,textarea,p,blockquote,th,td{margin:0;padding:0;}
address,caption,cite,code,dfn,em,strong,th,var{font-style:normal;}
ul{list-style:none;}
table{border-collapse:collapse;border-spacing:0;}
caption,th{text-align:left;}
q:before,q:after{content:'';}
object,embed{vertical-align:top;}
legend{display:none;}
h1,h2,h3,h4,h5,h6{font-size:100%;}
img,abbr,acronym,fieldset{border:0;}

#app {
  font-family: 'Noto Sans JP',Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

body{
  font: 14px/1.9 'Noto Sans JP', Arial, Verdana, 游ゴシック, YuGothic,'ヒラギノ角ゴ ProN W3', 'Hiragino Kaku Gothic ProN', メイリオ, Meiryo,sans-serif;
  -webkit-text-size-adjust:100%;
  overflow-x: hidden;
  color: #000;
  background: #fff;
  margin: 0;
  font-weight: 400;
}

section h2{
  padding: 50px 0 20px 0;
  font-size: 22px;
  text-align: center;
}
h1, h2, h3{
  font-family: 'Josefin Sans', 'Noto Sans JP',serif;
  font-weight: 600;
}
</style>
