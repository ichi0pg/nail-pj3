<template>
  <div>
    <Header />
    <div id="eyechatch">
      <img src="../assets/menu.jpg">
    </div>
    <div class="main">
      <div class="title">
        <div class="section-title">
          <img class="wing" src="../assets/line5.png" alt="CONCEPT">
          <h2>MENU</h2>
        </div>
      </div>
      <div class="menu">
        <div class="menu-wrap">
          <nav class="menu-nav">
            <ul>
              <li><a class="link2" @click="$router.push('/about')" >初めての方はこちら</a></li>
              <li><a class="link2" @click="scrollToAnchorPoint('gelmenu')">ジェルメニュー</a></li>
              <li><a class="link2" @click="scrollToAnchorPoint('careoff')">ケア＆オフ</a></li>
              <li><a class="link2" @click="scrollToAnchorPoint('other')">その他オプション</a></li>
            </ul>
          </nav>
          <div class="use-gel">
            <div class="use-wrap">
              <p class="menu-title">使用ジェル</p>
              <p><b>ベース＆トップジェル</b><br>KOKOIST ・ PREGEL<br><br><b>カラージェル</b><br>KOKOIST ・ PREGEL ・ Lily gel ・ VETRO ・ mao gel</p>
            </div>
          </div>
        </div>
      </div>
      <div class="title"  ref="gelmenu">
        <div class="section-title">
          <img class="wing" src="../assets/line5.png" alt="CONCEPT">
          <h2>GEL MENU</h2>
        </div>
      </div>
      <div class="gel-menu">
        <div class="gel-wrap">
          <div class="wrapper">
            <div class="menu1">
              <table class="table1">
                <tr>
                  <th class="menu-title">基本メニュー</th>
                </tr>
                <tr>
                  <th>・ハンドジェル</th><td>¥5,500</td>
                </tr>
                <tr>
                  <th>・フットジェル</th><td>¥6,500</td>
                </tr>
              </table>
            </div>
            <hr class="hr1">
            <div class="menu2">
              <table class="table2">
                <tr>
                  <th class="menu-title">定額ネイル&emsp;-ハンド-</th>
                </tr>
                <tr>
                  <th>・SIMPLE</th><td>¥6,000</td>
                </tr>
                <tr>
                  <th>・ART</th><td>¥7,000</td>
                </tr>
                <tr>
                  <th>・SPESIAL</th><td>¥8,500</td>
                </tr>
              </table>
            </div>
            <hr class="hr2">
            <hr class="hr3">
            <div class="menu3">
              <table class="table3">
                <tr>
                  <th class="menu-title">定額ネイル&emsp;-フット-</th>
                </tr>
                <tr>
                  <th>・SIMPLE</th><td>¥6,500</td>
                </tr>
                <tr>
                  <th>・ART</th><td>¥7,500</td> 
                </tr>
              </table>
            </div>
          </div>
        </div>
        <div class="memo">
          <p>※全てのメニュー、税抜き表示となっています。</p>
          <p>※定額ネイルはカラー、アート指の変更はできません。変更する場合は、別途料金¥100/1本がかかります。</p>
          <p>※デザイン、パーツ等の変更は通常の追加料金がかかります。</p>
        </div>
      </div>

      <div class="title" ref="careoff">
        <div class="section-title">
          <img class="wing" src="../assets/line5.png" alt="CONCEPT">
          <h2>CARE & OFF</h2>
        </div>
      </div>
      <div class="careoff">
        <div class="careoff-wrap">
          <div class="wrapper">
            <div class="menu1">
              <table class="table1">
                <tr>
                  <th class="menu-title">ケア</th>
                </tr>
                <tr>
                  <th>ハンドケア</th>
                </tr>
                <tr>
                  <th>・ウォーターケア</th><td>¥2,500</td>
                </tr>
                <tr><th>フットケア</th></tr>
                <tr>
                  <th>・ウォーターケア</th><td>¥3,500</td>
                </tr>
              </table>
            </div>
            <hr class="hr1">
            <div class="menu2">
              <table class="table2">
                <tr>
                  <th class="menu-title">オプション</th>
                </tr>
                <tr>
                  <th>・ハンドマッサージ</th><td>¥500</td>
                </tr>
                <tr>
                  <th>・フットマッサージ</th><td>¥500</td>
                </tr>
                <tr>
                  <th>・フットスクラブマッサージ</th><td>¥800</td>
                </tr>
                <tr>
                  <th>・足裏角質ケア</th><td>¥1,500</td>
                </tr>
              </table>
            </div>
            <hr class="hr4">
            <hr class="hr5">
            <div class="menu4">
              <table class="table4">
                <tr>
                  <th class="menu-title">オフ&emsp;＆&emsp;フィルイン</th>
                </tr>
                <tr>
                  <th>・1ヶ月以内&emsp;当店付け替え</th><td>無料</td>
                </tr>
                <tr>
                  <th>・1ヶ月以上&emsp;当店付け替え</th><td>¥200/1本</td>
                </tr>
                <tr>
                  <th>・他店オフ（溶剤オフのみ）</th><td>¥300/1本</td>
                </tr>
                <tr>
                  <th>・オフのみの方</th><td>¥300/1本</td> 
                </tr>
              </table>
            </div>
          </div>
        </div>
        <div class="memo">
          <p>※オプションは上記ケア料金にプラスになります。</p>
        </div>
      </div>

      <div class="title" ref="other">
        <div class="section-title">
          <img class="wing" src="../assets/line5.png" alt="CONCEPT">
          <h2>OTHER</h2>
        </div>
      </div>
      <div class="other">
        <div class="other-wrap">
          <div class="wrapper">
            <hr class="hr6">
            <div class="menu5">
              <table class="table5">
                <tr>
                  <th class="menu-title">長さだし</th>
                </tr>
                <tr>
                  <th>・アクリルスカルプチュア</th><td>1cmまで&emsp;¥500/1本</td>
                </tr>
                <tr>
                  <th style="font-size: 10px;">アクリルでアレルギーのある方は、ジェルで対応させていただきます。</th><td>1cm以上&emsp;¥800/1本</td>
                </tr>
              </table>
            </div>
            <hr class="hr7">
            <div class="menu6">
              <table class="table6">
                <tr>
                  <th class="menu-title">アートメニュー</th>
                </tr>
                <tr>
                  <th>・ラメフレンチ/逆フレンチ/マーブル/ラメ<br>ラメフレンチ/ラメグラデーション/ドット/ラインアート</th><td><br>¥200/1本</td>
                </tr>
                <tr>
                  <th>・2色までの簡単アート/カラーグラデーション<br>ベルベットシュガーミラーオーロラユニコーンマグネット</th><td><br>¥300/1本</td>
                </tr>
                <tr>
                  <th>・3色以上の奥行き感のないアート/ホワイトグラデーション</th><td>¥400/1本</td>
                </tr>
                <tr>
                  <th>・ニュアンスネイル<br>べっ甲、天然石などの奥行きのあるデザイン</th><td><br>¥500/本</td>
                </tr>
                <tr>
                  <th>・ネイルアーティストデザイン/ニットネイル</th><td>¥700/1本</td>
                </tr>
              </table>
            </div>
            <hr class="hr8">
            <div class="menu7">
              <table class="table7">
                <tr>
                  <th class="menu-title">その他アート・パーツ</th>
                </tr>
                <tr><th>・カラー/ラメライン</th><td>¥100</td></tr>
                <tr><th>・マットコート</th><td>¥150</td></tr>
                <tr><th>・ホロちらし</th><td>¥100</td></tr>
                <tr><th>・ホロ埋め尽くし</th><td>¥500</td> </tr>
                <tr><th>・3D/エンボス</th><td>¥300~</td></tr>
                <tr><th>・シール</th><td>¥100</td></tr>
                <tr><th>・ラメがけ</th><td>¥100</td></tr>
                <tr><th>・ラメちらし</th><td>¥50</td></tr>
                <tr><th>・フィルム（全体）</th><td>¥150</td></tr>
                <tr><th>・フィルム（ポイント）</th><td>¥50</td></tr>
                <tr><th>・スワロ&emsp;ss3~</th><td>¥50~</td></tr>
                <tr><th>・パール（半球）</th><td>¥50~</td></tr>
                <tr><th>・パール（球体）</th><td>¥50~</td></tr>
                <tr><th>・スタッズ</th><td>¥50</td></tr>
                <tr><th>・スワロVカット/スワロパール</th><td>¥50~</td></tr>
                <tr><th>・モチーフパーツ</th><td>¥50~</td></tr>
                <tr><th>・持ち込みパーツ埋め込み</th><td>¥150</td></tr>
                <tr><th>・金、銀箔ちらし</th><td>¥100</td></tr>
                <tr><th>・ラインテープ</th><td>¥10/1cm</td></tr>
                <tr><th>・ビジュー盛り</th><td>¥300/M¥400/L¥500</td></tr>
                <tr><th>・3Dスワロボール</th><td>S¥500/M¥1,000/L¥1,500</td></tr>
                <tr><th>・3D&emsp;NAIL&emsp;ART</th><td>¥800~</td></tr>
              </table>
            </div>
          </div>
        </div>
        <div class="memo">
          <p>※ジェルの基本料金に上記のアート、パーツ料金等がプラスになります。</p>
          <p>※パーツ・アートは1本、または1個あたりの料金になります。</p>
        </div>
      </div>
    </div>
    <div class="cat4">
      <img src="../assets/cat4.png" alt="cat1">
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
  },
  methods: {
    scrollToAnchorPoint(gelmenu) {
      const el = this.$refs[gelmenu]
      el.scrollIntoView({ behavior: 'smooth'})
    }
  }
};
</script>

<style>
body {
  font-size: 15px;
}
.gel-wrap {
  height: 30px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 5;
}
.wrapper {
  width: 85%;
  margin: auto;
}
.gel-nav ul {
  display: flex;
}
.gel-nav {
  margin-right: 30px;
  font-size: 14px;
}
a.gel-nav {
  list-style: none;
}
.menu,
.gel-menu,
.careoff,
.other {
  width: 100%;
  padding: 30px 0;
  margin: auto;
  background-color: #fff;
}
.menu {
  text-align: center;
}

.menu-wrap,
.gel-wrap,
.careoff-wrap,
.other-wrap {
  display: block;
  position: relative;
  width: 80%;
  margin: auto;
  padding: 25px 0;
  background-color: #fde3e5;
  border-radius: 50px;
}
.menu-wrap {
  height: fit-content;
}
.gel-wrap {
  height: 270px;
}
.careoff-wrap {
  height: 360px;
}
.other-wrap {
  height: 1150px;
}

.menu-nav ul {
  display: flex;
  width: 100%;
  margin: auto;
  justify-content: center;
}
.use-gel {
  margin-top: 20px;
}
.use-wrap p {
  padding-top: 10px;
  line-height: 2;
}
.menu1 {
  margin-bottom: 25px;
}
.menu3 {
  position: absolute;
  width: 50%;
  top: 160px;
  left: 58%;
}
.menu4 {
  position: absolute;
  width: 50%;
  top: 25px;
  left: 57%;
}
.menu5 {
  position: absolute;
  width: 80%;
  margin: auto;
}
.menu6 {
  position: absolute;
  width: 80%;
  top: 170px;
  margin: auto;
}
.menu7 {
  position: absolute;
  width: 80%;
  top: 470px;
  margin: auto;
}

/* メニュー表（テーブル） */
th {
  padding-bottom: 5px;
}
.table1,
.table2 {
  width: 40%;
}
.table3,
.table4 {
  width: 70%;
}
.table5,
.table6,
.table7 {
  width: 100%;
}
table tr {
  text-align: left;
}
table td {
  text-align: right;
}

/* 平行線 */
hr {
  width: 35%;
  background-color: #212020;
}
.hr1, .hr2, .hr3, .hr4,
.hr5, .hr6, .hr7, .hr8 {
  position: absolute;
}
.hr1 {
  top: 50px;
  left: 8%;
}
.hr2 {
  top: 185px;
  left: 8%;
}
.hr3 {
  top: 185px;
  right: 7%;
}
.hr4 {
  top: 240px;
  left: 8%;
}
.hr5 {
  width: 36%;
  top: 50px;
  right: 7%;
}
.hr6 {
  width: 80%;
  top: 50px;
}
.hr7 {
  width: 80%;
  top: 200px;
}
.hr8 {
  width: 80%;
  top: 500px;
}


.menu-title {
  padding-bottom: 20px;
  font-size: 18px;
}
p.menu-title {
  font-weight: bold;
}
.memo {
  width: 70%;
  margin: auto;
  padding-top: 20px;
  font-size: 12px;
}

/* 猫 */
.cat4 img {
  position: initial;
  width: 10%;
  margin-left: 15%;
  vertical-align: bottom;
}

@media screen and (max-width: 768px) {
  body {
    font-size: 14px;
  }
  .menu-nav ul {
    width: 80%;
  }
  .link2 {
    margin: 5px 15px;
    font-size: 12px;
  }

  .wrapper {
    width: 80%;
  }
  .menu2,
  .menu5 {
    padding-bottom: 25px;
  }
  .gel-wrap {
    height: 400px;
  }
  .careoff-wrap {
    height: 550px;
  }
  .other-wrap {
    height: 1070px;
  }

  .menu1, .menu2, .menu3, .menu4,
  .menu5, .menu6, .menu7, .menu8 {
    position: initial;
    width: 100%;
  }

  /* メニュー表（テーブル） */
  .table1, .table2, .table3,
  .table4, .table5, .table6, .table7 {
    width: 100%;
  }
  .table7 {
    margin-top: 20px;
  }

  /* 平行線 */
  hr {
    width: 80%;
  }
  .hr1 {
    left: initial;
  }
  .hr2 {
    top: 185px;
    left: initial;
  }
  .hr3 {
    top: 345px;
    right: initial;
  }
  .hr4 {
    top: 240px;
    left: initial;
  }
  .hr5 {
    width: 80%;
    top: 430px;
    right: initial;
  }
  .hr7 {
    top: 185px;
  }
  .hr8 {
    top: 460px;
  }
  /* 猫 */
  .cat4 img {
    left: 20px;
    bottom: -110px;
    object-fit: contain;
  }
}

@media screen and (max-width: 480px) {
  body {
    font-size: 11px;
  }
  .menu-nav {
    display: none;
  }
  .menu-wrap {
    height: 150px;
    border-radius: 25px;
  }
  .gel-wrap,
  .careoff-wrap,
  .other-wrap {
    border-radius: 25px;
  }
  .gel-wrap {
    height: 300px;
  }
  .careoff-wrap {
    height: 400px;
  }
  .other-wrap {
    height: 970px;
  }
  .menu-title {
    font-size: 12px;
  }
  .use-wrap p {
    padding-top: initial;
  }
  .use-gel {
    margin-top: initial;
  }
  /* メニュー表（テーブル） */
  th {
    width: 70%;
    padding-bottom: 3px;
  }

  /* 平行線 */
  hr {
    width: 80%;
  }
  .hr1 {
    top: 45px;
    left: initial;
  }
  .hr2 {
    top: 150px;
    left: initial;
  }
  .hr3 {
    top: 275px;
    right: initial;
  }
  .hr4 {
    top: 190px;
    left: initial;
  }
  .hr5 {
    width: 80%;
    top: 335px;
    right: initial;
  }
  .hr6 {
    top: 45px;
  }
  .hr7 {
    top: 175px;
  }
  .hr8 {
    top: 495px;
  }
  .menu-title {
    padding-bottom: 15px;
  }
  .memo {
    font-size: 10px;
  }
  /* 猫 */
  .cat4 img {
    width: 13%;
  }
}
</style>