<template>
  <div id="app">
    <Header></Header>
    <div class="page-mv">
      <h1 class="ttl">事業内容</h1>
    </div>
    <!-- page-mv end -->
    <main>
      <div class="service ptb-m wrap">
        <div class="service-list">
          <section class="service-item">
            <div class="service-item-img">
              <img src="img/service1.png" alt="IT人材育成事業">
            </div>
            <div class="service-item-detail">
              <h2 class="service-item-ttl">IT人材育成事業</h2>
              <p class="service-item-depiction">これまでに培った教育手法を生かして、短期間で即戦力のIT人材を育成します。</p>
            </div>
          </section>
          <section class="service-item">
            <div class="service-item-img">
              <img src="img/service2.png" alt="コーチング事業">
            </div>
            <div class="service-item-detail">
              <h2 class="service-item-ttl">コーチング事業</h2>
              <p class="service-item-depiction">目標達成を最短で実現するために、プロのコーチによるマンツーマンのサポートを実施します。</p>
            </div>
          </section>
          <section class="service-item">
            <div class="service-item-img">
              <img src="img/service3.png" alt="ITコンサル事業">
            </div>
            <div class="service-item-detail">
              <h2 class="service-item-ttl">ITコンサル事業</h2>
              <p class="service-item-depiction">経営戦略にIT戦略を策定し、システム開発の提案やシステムの最適化を通じて、企業の経営をサポートします。</p>
            </div>
          </section>
          <section class="service-item">
            <div class="service-item-img">
              <img src="img/service4.png" alt="デジタルトランスフォーメーション事業">
            </div>
            <div class="service-item-detail">
              <h2 class="service-item-ttl">デジタルトランスフォーメーション事業</h2>
              <p class="service-item-depiction">人々の生活をよりよいものに変革するために様々なデジタル技術を活用し、革新的なソリューションやサービスを生み出します。</p>
            </div>
          </section>
        </div>
      </div>
    </main>
    <!-- bottom-contact-->
    <section class="bottom-contact ptb-m">
      <div class="wrap">
        <h2 class="bottom-contact-ttl ttl">お問い合わせ</h2>
        <p class="bottom-contact-txt">
          お仕事のご依頼や採用に関してはお問い合わせにて承っております。
        </p>
        <a href="contact.html" class="bottom-contact-btn btn btn-primary">お問い合わせ</a>
      </div>
    </section>
    </div>
</template>


<script>
import Header from "./components/Header";
export default{
  components:{
    Header
  }
};
</script>

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

/* change colours to suit your needs */
ins {
  background-color:#ff9;
  color:#000;
  text-decoration:none;
}

/* change colours to suit your needs */
mark {
  background-color:#ff9;
  color:#000;
  font-style:italic;
  font-weight:bold;
}

del {
  text-decoration: line-through;
}

abbr[title], dfn[title] {
  border-bottom:1px dotted;
  cursor:help;
}

table {
  border-collapse:collapse;
  border-spacing:0;
}

/* change border colour to suit your needs */
hr {
  display:block;
  height:1px;
  border:0;
  border-top:1px solid #cccccc;
  margin:1em 0;
  padding:0;
}

input, select {
  vertical-align:middle;
}
.service-item{
	padding: 20px 0;
	border-top: 1px solid #222;
	display: flex;
	flex-wrap: wrap;
	justify-content: space-between;
}

.service-item:last-child{
	border-bottom: 1px solid #222;
}

.service-item-img{
	width: 290px;
}

.service-item-detail{
	width: calc(100% - 330px);
}

.service-item-ttl{
	font-size: 24px;
	font-weight: bold;
}

@media screen and (max-width: 768px){
  .service-item-detail{
    width: 100%;
  }

  .service-item-img{
    width: 100%;
  }
}
</style>
