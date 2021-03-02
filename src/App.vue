<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style>
html, body, div, span, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
abbr, address, cite, code,
del, dfn, em, img, ins, kbd, q, samp,
small, strong, sub, sup, var,
b, i,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, figcaption, figure,
footer, header, hgroup, menu, nav, section, summary,
time, mark, audio, video {
  margin:0;
  padding:0;
  border:0;
  outline:0;
  font-size:100%;
  vertical-align:baseline;
  background:transparent;
}
body {
  line-height:1;
}
article,aside,details,figcaption,figure,
footer,header,hgroup,menu,nav,section {
  display:block;
}
nav ul {
  list-style:none;
}
blockquote, q {
    quotes:none;
}

blockquote:before, blockquote:after,
q:before, q:after {
    content:'';
    content:none;
}
a {
  margin:0;
  padding:0;
  font-size:100%;
  vertical-align:baseline;
  background:transparent;
}

body {
  background-color: rgba(250, 198, 203, 0.48);
  color: #333;
  font-size: 16px;
  font-family: 'Sen', sans-serif;
  line-height: 1.5;
}
h1, h2,
.copyright {
 font-family: 'Sofia', cursive;
}
h1 {
  width: 100%;
  text-align: center;
  font-size: 4vw;
  font-weight: initial;
  color: #fff;
}
h2 {
  text-align: center;
  margin-bottom: 10px;
  font-size: 20px;
  color: #333;
}
h3 {
  text-align: center;
  margin-bottom: 10px;
  font-size: 16px;
  color: #333;
}
.wing {
  position: absolute;
  width: 25%;
  left: 0;
  right: 0;
  margin: auto;
}
.wing2 {
  position: absolute;
  width: 45%;
  left: 0;
  right: 0;
  margin: auto;
}

.header {
  position: fixed;
  width: 100%;
  z-index: 100;
}
#eyechatch img {
  width: 100%;
  object-fit: cover;
  object-position: 50% 100%;
  vertical-align: bottom;
}
.link {
  margin-left: 50px;
  color: #fac6cb;
  cursor: pointer;
  text-decoration: none;
}
.link2 {
  margin: 10px 30px;
  color: #444343;
  cursor: pointer;
  text-decoration: none;
}
.title {
  position: relative;
  height: 40px;
  margin-top: 40px;
  margin-bottom: 15px;
}
.section-title {
  text-align: center;
}
/* 猫 */
.cat {
  width: 100%;
}

@media screen and (max-width: 768px) {
  body {
    font-size: 12px;
  }
  h1 {
    font-size: 6vw;

    font-weight: initial;
  }
  h2 {
    font-size: 17px;
    font-weight: initial;
  }
  h3 {
    font-size: 14px;
  }
  .wing {
    width: 30%;
  }
  .wing2 {
    width: 55%;
  }

  #eyechatch {
    background-image: initial;
    height: initial;
    margin-bottom: initial;
  }
  #eyechatch img {
    max-width: 100%;
    height: auto;
  }
  .title {
    margin-top: 40px;
  }

}
@media screen and (max-width: 480px) {
  body {
    font-size: 11px;
  }
  h2 {
    font-size: 12px;
  }
  
  .title {
    margin-top: 25px;
    margin-bottom: 0;
  }
  .wing {
    width: 35%;
  }
  .wing2 {
    width: 65%;
  }
  .main-title {
    font-size: 14px;
  }
}
</style>