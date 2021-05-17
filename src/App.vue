<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style>
@import url(http://fonts.googleapis.com/earlyaccess/notosansjp.css);
@import url(https://fonts.googleapis.com/css?family=Pacifico);

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
  font-family: Avenir, Helvetica, Arial, sans-serif;
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

body {
  margin: 0;
}

section h2{
  padding: 50px 0 20px 0;
  font-size: 22px;
  font-weight:normal;
  text-align: center;
}
h1, h2{
  font-family: 'Josefin Sans', 'Noto Sans JP',serif;
}
</style>
