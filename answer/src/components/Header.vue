  <template>
  <header class="header">
      <h1 class="header-ttl">
        <a href="index.html">
          TECH
        </a>
      </h1>
      <nav class="header-nav">
        <ul class="header-nav-list">
          <li class="header-nav-item"><a href="App.vue">ホーム</a></li>
          <li class="header-nav-item"><a href="service.html">事業内容</a></li>
          <li class="header-nav-item"><a href="news.html">ニュース</a></li>
          <li class="header-nav-item"><a href="blog.html">社員ブログ</a></li>
          <li class="header-nav-item"><a href="company.html">会社概要</a></li>
          <li class="header-nav-item"><a href="recruit.html">採用情報</a></li>
          <li class="header-nav-item"><a href="contact.html">お問い合わせ</a></li>
        </ul>
      </nav>
      <div class="menu" id="menu" @click="hamburger()" :class="{'active':isClass}">
        <span class="menu-line-top"></span>
        <span class="menu-line-middle"></span>
        <span class="menu-line-bottom"></span>
      </div>
      <nav class="drawer-nav" id="drawer-nav" :class="{'open':isClass}">
        <p class="menu-title">TECH</p>
        <ul class="drawer-nav-list">
          <li class="drawer-nav-item"><a href="index.html">ホーム</a></li>
          <li class="drawer-nav-item"><a href="service.html">事業内容</a></li>
          <li class="drawer-nav-item"><a href="news.html">ニュース</a></li>
          <li class="drawer-nav-item"><a href="blog.html">社員ブログ</a></li>
          <li class="drawer-nav-item"><a href="company.html">会社概要</a></li>
          <li class="drawer-nav-item"><a href="recruit.html">採用情報</a></li>
          <li class="drawer-nav-item"><a href="contact.html">お問い合わせ</a></li>
        </ul>
      </nav>
    </header>
</template>

<script>
export default{
  data(){
    return{
      isClass:false
    };
  },
  methods:{
    hamburger(){
      this.isClass=!this.isClass;
    }
  }
};
</script>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 70px;
  padding: 0 30px;
  background-color: #fff;
  position: sticky;
  left: 0;
  top: 0;
  z-index: 1;
}

.header-ttl {
  font-size: 24px;
  width: 80px;
}
.header-ttl a{
  text-decoration:none;
  color:black;
}

.header-nav-list {
  display: flex;
  font-weight: bold;
  list-style:none;
  }
.header-nav-item a{
  text-decoration: none;
  color: black;
}
.header-nav-item:not(:last-child) {
  margin-right: 30px;
}

.menu {
  display: none;
}
.drawer-nav {
  display: none;
}

@media screen and (max-width:768px){
   .wrap {
    width: 85%;
  }

  .wrap-s {
    width: 90%;
  }

  .header-nav {
    display: none;
  }

  .menu {
    display: inline-block;
    width: 36px;
    height: 32px;
    cursor: pointer;
    position: relative;
    z-index: 10;
  }

  .menu-line-top,
  .menu-line-middle,
  .menu-line-bottom {
    display: inline-block;
    width: 100%;
    height: 4px;
    background-color: #000;
    position: absolute;
    transition: 0.5s;
  }

  .menu-line-top {
    top: 0;
  }

  .menu-line-middle {
    top: 14px;
  }

  .menu-line-bottom {
    bottom: 0;
  }

  .menu.active span:nth-of-type(1) {
    top: 14px;
    transform: rotate(45deg);
  }

  .menu.active span:nth-of-type(2) {
    opacity: 0;
  }

  .menu.active span:nth-of-type(3) {
    top: 14px;
    transform: rotate(-45deg);
  }
  .drawer-nav{
    display: block;
    position: absolute;
    height: 100vh;
    width: 100%;
    top: 0;
    left: -100%;
    background: #fff;
    transition: .7s;
  }

  .drawer-nav-list {
    padding-top: 80px;
    text-align: center;
    list-style:none;
  }
.drawer-nav-list a{
  text-decoration: none;
  color: black;
}
  .drawer-nav-item {
    margin-top: 40px;
    color: #0033cc;
    font-size: 18px;
  }
.drawer-nav.open{
  left:0;
}
}
</style>