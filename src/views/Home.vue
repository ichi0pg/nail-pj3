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
            <div class="about-left">
              <img class="img1" src="../assets/about-home.jpg" alt="ABOUT">
              <img class="img2" src="../assets/about.home.jpg" alt="ABOUT">
              <div class="about-button">
                <button class="btn-link" @click="$router.push('/about')">read more</button>
              </div>
            </div>
            <div class="menu-right">
              <img class="img1" src="../assets/menu-home.jpg" alt="MENU">
              <img class="img2" src="../assets/menu.home.jpg" alt="MENU">
              <div class="menu-button">
                <button class="btn-link" @click="$router.push('/menu')">read more</button>
              </div>
            </div>
          </div>
          <div class="order2">
            <div class="title">
              <div class="section-title">
                <img class="wing" src="../assets/line5.png" alt="CONCEPT">
                <h1>CONCEPT</h1>
                <div class="con">
                  <p>指先が綺麗だと、自慢したくなる。<br>指先が綺麗だと、気分も上がる。<br>指先が綺麗になると、仕草も変わる。<br><br>何をする時でも指先は自然と視界に入ります。<br>ネイルをすることで爪も丈夫になり、物を扱う仕草や手の扱い方も綺麗になります。<br><br>是非指先から綺麗になるお手伝いをさせてください。</p>
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
            <img src="../assets/insta.png" alt="">
          </div>
        </div>
        <div class="right-img">
          <img src="../assets/prf.con.jpg" alt="PROFILE_CONTACT">
          <div class="last-btn">
            <button class="btn-right" @click="$router.push('/profile')">read more</button>
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
.about-left img {
  width: 100%;
  position: relative;
}
.menu-right img {
  width: 100%;
  position: relative;
}
.about-left p {
  position: absolute;
  top: 50%;
  width: 50%;
}
.menu-right p {
  position: absolute;
  top: 50%;
  width: 50%;
}
.about-left p,
.menu-right p {
  text-align: center;
  color: #fff;
  font-size: 50px;
}
.about-button,
.menu-button {
  text-align: center;
  position: absolute;
  width: 50%;
  top: 30%;
}
.btn-link {
  padding: 5px 15px;
  text-decoration: none;
  background-color: rgba(255, 255, 255, 0.3);
  border-radius: 10px;
  cursor: pointer;
  border: none;
  color: #fff;
  font-size: 18px;
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
  padding-left: 45px;
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
.sns-link img {
  position: absolute;
  width: 25px;
  left: 10px;
}
.right-img img {
  position: absolute;
  width: 55%;
  bottom: -130px;
  right: 0;
}
.last-btn {
  position: absolute;
  bottom: -40px;
  right: 25%;
}
.btn-right {
  padding: 5px 15px;
  text-decoration: none;
  background-color: rgba(255, 255, 255, 0.3);
  border-radius: 10px;
  cursor: pointer;
  border: none;
  font-size:18px;
  color: #fff;
}
.cat1 img {
  width: 10%;
  left: 5%;
  bottom: -140px;
  object-fit: contain;  
}

@media screen and (max-width: 768px) {
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
  .about-left,
  .menu-right {
    height: 280px;
  }
  .about-left img,
  .menu-right img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  .about-left p {
    width: 100%;
    top: 20%;
    font-size: 32px;
  }
  .menu-right p {
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
  .btn-link,
  .btn-right {
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
    margin-bottom: 100px;
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
  .sns-link img {
    width: 22px;
  }
  a.btn-sns {
    padding-left: 40px;
    font-size: 14px;
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
  .cat1 img {
    width: 15%;
    height: 15%;
    bottom: -115px;
    object-fit: contain;
  }
}

@media screen and (max-width: 480px) {
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
  .about-left,
  .menu-right {
    height: 150px;
  }
  .about-left img,
  .menu-right img{
    vertical-align: bottom;
  }
  .about-button {
    top: 65%;
  }
  .menu-button {
    top: 90%;
  }
  .btn-link,
  .btn-center,
  .btn-right {
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
  .sns-link img {
    width: 20px;
    left: 38%;
  }
  a.btn-sns {
    position: relative;
    top: 0px;
    font-size: 12px;
  }
  .last-btn {
    bottom: 30px;
  }
  .cat1 img {
    bottom: -130px;
  }
}
</style>