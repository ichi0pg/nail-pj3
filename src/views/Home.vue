<template>
  <div>
    <Header />
    <div id="eyechatch">
      <img src="../assets/main.jpg" alt="HOME">
    </div>
    <div class="main">
      <div class="main-wrap">
        <div class="set">
          <div class="order1">
            <div class="contents-left">
              <img src="../assets/about-home.jpg" alt="ABOUT">
              <h1 class="top-title2">ABOUT</h1>
              <div class="about-button">
                <button class="link-btn" @click="$router.push('/about')">read more</button>
              </div>
            </div>
            <div class="contents-right">
              <img src="../assets/menu-home.jpg" alt="MENU">
               <h1 class="top-title3">MENU</h1>
              <div class="menu-button">
                <button class="link-btn" @click="$router.push('/menu')">read more</button>
              </div>
            </div>
          </div>
          <div class="order2">
            <div class="title">
              <div class="section-title">
                <img class="wing" src="../assets/line5.png" alt="CONCEPT">
                <h2>CONCEPT</h2>
                <div class="con">
                  <p>指先が綺麗だと、気分が上がる。<br>指先が綺麗だと、自慢したくなる。<br>指先が綺麗になると、仕草も変わる。<br><br>何をする時でも指先は自然と視界に入ります。<br>ネイルをすることで爪も丈夫になり<br>物を扱う仕草や手の扱い方も綺麗になり<br>より女性らしい仕草になっていきます。<br><br>是非指先から綺麗になるお手伝いをさせてください。</p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="sub-menu">
      <div class="sub-wrap">
        <div class="back-color">
          <div class="instagram">
            
          </div>
          <div class="sns-link">
            <a @click="$router.push('/')" class="btn-sns">Instagram</a>
          </div>
        </div>
        <div class="right-img">
          <img src="../assets/prf-con.jpg" alt="PROFILE_CONTACT">
          <h1 class="top-title4">PROFILE & CONTACT</h1>
          <div class="last-btn">
            <button class="link-btn" @click="$router.push('/profile')"><span>read more</span></button>
          </div>
          <div class="cat1">
            <img src="../assets/cat2.png" alt="cat1">
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "../components/Header";
import Footer from "../components/Footer";
export default {
  components: {
    Header,
    Footer
  }
};
</script>

<style>
.top-title2,
.top-title3 {
  position: absolute;
  width: 50%;
  top: 15%;
  margin: auto;
}
.top-title4 {
  position: absolute;
  width: 55%;
  bottom: 10%;
  right: 0;
  margin: auto;
  font-size: initial;
  font-size: 4vw;
}
/* main-wrap */
.main-wrap {
  position: relative;
}
.set {
  display: flex;
  flex-direction: column;
}
.order1 {
  display: flex;
}
.order2 {
  height: 370px;
}
.contents-left img {
  width: 100%;
  position: relative;
}
.contents-right img {
  width: 100%;
  position: relative;
}
.contents-left p {
  position: absolute;
  top: 50%;
  width: 50%;
}
.contents-right p {
  position: absolute;
  top: 50%;
  width: 50%;
}
.contents-left p,
.contents-right p {
  text-align: center;
  color: #fff;
  font-size: 50px;
}
.about-button,
.menu-button {
  text-align: center;
  position: absolute;
  width: 50%;
  top: 35%;
}
.link-btn {
  color: #fff;
  border: 2px solid #fff;
  border-radius: 0;
  background-image: -webkit-gradient(linear, left top, right top, from(#fa709a), to(pink
  ));
  background-image: -webkit-linear-gradient(left, #fa709a 0%, pink 100%);
  background-image: linear-gradient(to right, #fa709a 0%, pink 100%);
  -webkit-box-shadow: 0 5px 10px rgba(0, 0, 0, .1);
  box-shadow: 0 5px 10px rgba(0, 0, 0, .1);
}
.link-btn:hover {
  -webkit-transform: translate(0, -2px);
  transform: translate(0, -2px);
  color: #fff;
  -webkit-box-shadow: 0 8px 15px rgba(0, 0, 0, .3);
  box-shadow: 0 8px 15px rgba(0, 0, 0, .3);
}

/* concept */
.con p {
  position: absolute;
  top: 70px;
  left: 0;
  right: 0;
}

/* sub-menu */
.sub-menu {
  position: relative;
}
.sub-wrap {
  height: 450px;
  background-color: #fff;
  margin-bottom: 130px;
}
a.btn-sns {
  padding-top: 5px;
  padding-bottom: 5px;
  padding-left: 15px;
  padding-right: 15px;
  color: #444343;
  background-color: #fce3e5;
  text-decoration: none;
  border: 1.7px #444343 solid;
  font-size: 18px;
}
.sns-link {
  position: relative;
  width: 40%;
  left: 18%;
  top: 380px;
}
.right-img img {
  position: absolute;
  width: 55%;
  bottom: -130px;
  right: 0;
}
.last-btn {
  position: absolute;
  width: 55%;
  bottom: -40px;
  right: 0;
  text-align: center;
}
.link-btn {
  padding: 5px 15px;
  text-decoration: none;
  background-color: rgba(255, 255, 255, 0.3);
  border-radius: 10px;
  cursor: pointer;
  border: none;
  font-size:18px;
  color: #fff;
}
/* 猫 */
.cat1 img {
  width: 10%;
  left: 5%;
  bottom: -140px;
  object-fit: contain;  
}

@media screen and (max-width: 768px) {
  .top-title2 {
    position: absolute;
    width: 100%;
    top: 50%;
    text-align: center;
  }
  .top-title3 {
    position: absolute;
    width: 100%;
    top: 80%;
    text-align: center;
  }
  .top-title4 {
    position: absolute;
    width: 100%;
    bottom: 15%;
    font-size: 5vw;
  }
  /* main-wrap */
  .main-wrap {
    margin-bottom: initial;
  }
  .order1 {
    order: 2;
    flex-wrap: wrap;
  }
  .order2 {
    order: 1;
    height: 350px;
  }
  .order2 p {
    width: 80%;
    margin: auto;
  }
  .con p {
    top: 50px;
  }
  .contents-left,
  .contents-right {
    height: 280px;
  }
  .contents-left img,
  .contents-right img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  .contents-left p {
    width: 100%;
    top: 20%;
    font-size: 32px;
  }
  .contents-right p {
    width: 100%;
    top: 70%;
    font-size: 32px;
  }
  .about-button {
    width: 100%;
    top: 58%;
  }
  .menu-button {
    width: 100%;
    top: 89%;
  }
  .con-button {
    top: 245px;
  }
  .btn-center,
  .link-btn {
    font-size: 14px;
  }

  /* sub-menu */
  .last-title {
    width: 100%;
    height: 30%;
    font-size: 24px;
  }
  .sub-wrap {
    background-color: initial;
    height: 850px;
    margin-bottom: 130px;
  }
  .sns-wrap p {
    color: #000;
  }
  .back-color {
    position: absolute;
    width: 100%;
    height: 400px;
    top: 47px;
    background-color: #fff;
  }
  .sns-link {
    top: 350px;
    left: 40%;
  }
  a.btn-sns {
    font-size: 12px;
  }
  .right-img img {
    width: 100%;
    height: 40%;
    bottom: 0;
    object-fit: cover;
  }
  .last-btn {
    left: initial;
    right: initial;
    width: 100%;
    bottom: 80px;
    text-align: center;
  }
  /* 猫 */
  .cat1 img {
    width: 15%;
    height: 15%;
    bottom: -145px;
    object-fit: contain;
  }
}

@media screen and (max-width: 480px) {
  .top-title2 {
    top: 55%;
  }
  .top-title4 {
    bottom: 12%;
  }
  /*consept*/
  .order2 {
    height: 280px;
  }
  .con p {
    top: 45px;
  }
  .con-button {
    top: 200px;
  }
  .contents-left,
  .contents-right {
    height: 150px;
  }
  .contents-left img,
  .contents-right img{
    vertical-align: bottom;
  }
  .about-button {
    top: 65%;
  }
  .menu-button {
    top: 90%;
  }
  .link-btn,
  .btn-center,
  .link-btn {
    font-size: 10px;
  }

  /* sub-wrap */
  .sub-wrap {
    height: 660px;
    margin-bottom: 58px;
  }
  .back-color {
    top: 30px;
  }
  .right-img img {
    height: 30%;
  }
  .sns-link {
    left: initial;
    width: 100%;
    text-align: center;
  }
  a.btn-sns {
    position: relative;
    top: 0px;
    font-size: 11px;
  }
  .last-btn {
    bottom: 30px;
  }
  /* 猫 */
  .cat1 img {
    bottom: -133px;
  }
}
</style>