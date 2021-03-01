<template>
  <div>
    <Header />
    <div id="eyechatch">
      <img src="../assets/prf.jpg">
    </div>
    <div class="main">
      <div class="title">
        <div class="section-title">
          <img class="wing2" src="../assets/line1.png" alt="CONCEPT">
          <h1>PROFILE</h1>
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
            <h1>CONTACT</h1>
          </div>
        </div>
        <div class="second-wrap">
          <div class="wrap2">
            <div class="res-left">
              <h2>予約ついて</h2>
              <p class="reserve">土日限定<br>予約時間9:00~14:00<br><br>仕事などの関係で希望日に予約がとれない場合があります。<br><br>18:00までには終わらせたいので、時間に縛りはありませんがデザイン等悩まれる方は、時間にゆとりを持って予約をしていただくようにお願いします。</p>
            </div>
          </div>
          <div class="wrap2">
            <div class="acc-right">
              <h2>ACCESS</h2>
              <p class="access">豊田市<br>敷地内に駐車場があります。<br><br>車高が低い、長さがある車は入って来られないかもしれません。<br><br>電車などでお越しの場合は駅までお迎えに行くので、予約の際に教えてください。<br><br>実家なので、詳細な住所はLINEにてご連絡させていただきます。</p>
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
.img2 {
  display: none;
}
.section-title {
  text-align: center;
}

.prf-wrap {
  display: flex;
  position: relative;
  width: 90%;
  height: 420px;
  margin: auto;
  background-color: #fff;
  border-radius: 50px;
}
.prf-left {
  width: 300px;
}
.prf-img {
  height: 350px;
  object-fit: cover;
  margin: 35px;
  border-radius: 50px;
}
.wrap {
  width: 60%;
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
  top: 50%;
  transform: translateY(-50%);
  left: 40%;
  font-size: 14px;
}
.prf-right p {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  left: 65%;
  font-size: 14px;
  line-height: 2em;
}

.second-wrap {
  position: relative;
  display: flex;
  width: 90%;
  height: 400px;
  margin: auto;
  border-radius: 50px;
  background-color: #fff;
}
.res-left,
.acc-right {
  width: 80%;
  height: 260px;
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
  font-size: 14px;
}
.cat {
  width: 100%;
  text-align: right;
}
.cat2 img {
  position: initial;
  width: 10%;
  margin-left: 85%;
  vertical-align: bottom;
}

@media screen and (max-width: 768px) {
  .img2 {
    display: initial;
  }
  .img1{
    display: none;
  }
  .prf-wrap {
    width: 80%;
    height: 800px;
  }
  .second-wrap {
    display: block;
    height: fit-content;
    width: 80%;
  }
  .prf-left {
    width: 50%;
  }
  .prf-center p {
    top: 20%;
    transform: translateY(-20%);
    left: 60%;
    font-size: initial;
  }
  .prf-right p {
    width: 100%;
    top: 93%;
    left: 0;
    right: 0;
    transform: translateY(-100%);
    text-align: center;
    font-size: initial;
  }
  .prf-img {
    width: 100%;
    height: 45%;
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
  }
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
    margin-bottom: 0;
    border-radius: 25px;
  }
  .wrap {
    background-color: initial;
    height: initial;
  }
  .prf-left {
    width: 100%;
  }
  .prf-center p {
    width: 40%;
    top: 10%;
    left: 50%;
    transform: translateY(-10px);
    font-size: 10px;
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
    height: auto;
    margin: auto;
    padding-bottom: 25px;
    border-radius: 50px;
    background-color: #fff;
 }
 .res-left,
 .acc-right {
   background-color: initial;
   width: 80%;
 }
 .res-left p,
 .acc-right p {
   font-size: 11px;
 }
 .res-left p {
   padding-bottom: 10px;
 }
 .cat2 img {
    width: 15%;
    margin-left: 80%;
  }
}
</style>