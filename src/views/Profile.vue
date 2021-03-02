<template>
  <div>
    <Header />
    <div id="eyechatch">
      <img src="../assets/prf.jpg">
      <h1 class="top-title5">PROFILE & CONTACT</h1>
    </div>
    <div class="main">
      <div class="title">
        <div class="section-title">
          <img class="wing2" src="../assets/line1.png" alt="CONCEPT">
          <h2>PROFILE</h2>
        </div>
      </div>
      <div class="prf-menu">
        <div class="prf-wrap">
          <div class="prf-left">
            <img class="prf-img"  src="../assets/prf.png" alt="profile">
          </div>
          <div class="wrap">
            <div class="prf-center">
              <p class="name">裕代<br><br>ネイリスト<br><br>1988/05/17<br>O型<br><br>猫ちゃん、ドライブ、ゲーム<br>漫画、アニメ好きです。<br><br></p>
            </div>
            <div class="prf-right">
              <p class="name">JNEC ネイリスト検定 1級<br>JNA ジェルネイル検定 上級<br>ネイルサロン衛生管理士<br>KOKOIST Meister<br>VETRO TECHNICIAN<br>3D NAIL ART Traning Program 1,2 他<br><br>Nailist ネイルスクール<br>インストラクター養成コース卒業</p>
            </div>
          </div>
        </div>
      </div>           
      <div class="con-menu">
        <div class="title">
          <div class="section-title">
            <img class="wing2" src="../assets/line1.png" alt="contact">
            <h2>CONTACT</h2>
          </div>
        </div>
        <div class="second-wrap">
          <div class="wrap2">
            <div class="res-left">
              <h3>予約ついて</h3>
              <p class="reserve"><b>土日限定<br>予約時間9:00~14:00</b><br><br>仕事などの関係で希望日に予約がとれない場合があります。<br><br>18:00までには終わらせたいので、時間に縛りはありませんがデザイン等悩まれる方は、時間にゆとりを持って予約をしていただくようにお願いします。</p>
            </div>
          </div>
          <div class="wrap2">
            <div class="acc-right">
              <h3>ACCESS</h3>
              <p class="access"><b>豊田市</b><br>敷地内に駐車場があります。<br><br>車高が低い、長さがある車は入って来られないかもしれません。<br><br>電車などでお越しの場合は駅までお迎えに行くので、予約の際に教えてください。<br><br>実家なので、詳細な住所はLINEにてご連絡させていただきます。</p>
            </div>
          </div>
        </div>
        <div class="cat2">
          <img src="../assets/cat1.png" alt="cat2">
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
.top-title5 {
  position: absolute;
  bottom: 10%;
}
.section-title {
  text-align: center;
}
.prf-wrap {
  display: flex;
  width: 80%;
  height: 500px;
  margin: auto;
  background-color: #fff;
  border-radius: 50px;
}
.prf-img {
  width: 100%;
  height: 80%;
  object-fit: cover;
  margin: 45px;
  border-radius: 50px;
}
.wrap {
  position: relative;
  width: 50%;
  height: 80%;
  margin: auto;
  background-color: #fce3e5;
  border-radius: 50px;
}
.wrap2 {
  width: 50%;
  margin: auto;
}

.prf-center p {
  position: absolute;
  width: 35%;
  top: 55px;
  left: 30px;
}
.prf-right p {
  position: absolute;
  width: 45%;
  top: 45px;
  left: 50%;
}
.prf-left {
  width: 30%;
}

.second-wrap {
  position: relative;
  display: flex;
  width: 80%;
  height: 550px;
  margin: auto;
  border-radius: 50px;
  background-color: #fff;
}
.res-left,
.acc-right {
  width: 75%;
  height: 350px;
  margin: auto;
  padding: 20px;
  border-radius: 50px;
  background-color: #fce3e5;
}
.res-left p,
.acc-right p {
  width: 80%;
  margin: auto;
  margin-top: 20px;
}

/* 猫 */
.cat2 img {
  position: initial;
  width: 10%;
  margin-left: 85%;
  vertical-align: bottom;
}

@media screen and (max-width: 768px) {
  .prf-wrap {
    width: 80%;
    height: 700px;
  }
  .second-wrap {
    display: block;
    height: fit-content;
    width: 80%;
  }
  .prf-img {
    width: 100%;
    height: 45%;
    margin-left: 20px;
    border-radius: 25px;
  }
  .prf-left {
    width: 40%;
  }
  .prf-center p {
    top: 30px;
    width: 70%;
  }
  .prf-right p {
    width: 100%;
    top: 100%;
    left: -40%;
    transform: translateY(-100%);
    text-align: center;
  }

  .wrap {
    background-color: initial;
  }
  .wrap2 {
    width: 80%;
    padding-top: 10px;
    padding-bottom: 20px;
  }
  .res-left,
  .acc-right {
    background-color: initial;
    height: fit-content;
  }
  .res-left p,
  .acc-right p {
    width: 100%;
    margin-top: 30px;
    font-size: 1vh;
  }
  /* 猫 */
  .cat2 img {
    width: 10%;
    height: 13%;
    left: 20px;
    bottom: -110px;
    object-fit: contain;
  }
}

@media screen and (max-width: 480px) {
  .prf-wrap {
    flex-wrap: wrap;
    width: 85%;
    height: 480px;
    border-radius: 25px;
  }
  .prf-img {
    width: 35%;
    height: 75%;
    margin: 25px;
    border-radius: 20px;
  }
  .wrap {
    background-color: initial;
    height: initial;
    width: 80%;
  }
  .prf-left {
    width: 100%;
  }
  .prf-center p {
    width: 45%;
    top: -130%;
    left: 50%;
    transform: translateY(-10px);
  }
  .prf-right {
    text-align: center;
    margin: 20px;
  }
  .prf-right p {
    position: initial;
    margin: auto;
    top: 10%;
    transform: translateY(-10px);
    font-size: 10px;
  }
 .second-wrap {
    width: 85%;
    height: auto;
    margin: auto;
    padding-bottom: 25px;
    border-radius: 25px;
    background-color: #fff;
 }
 .res-left,
 .acc-right {
   background-color: initial;
   width: 80%;
 }
 .res-left p {
   padding-bottom: 10px;
 }
 /* 猫 */
 .cat2 img {
    width: 15%;
    margin-left: 80%;
  }
}
</style>