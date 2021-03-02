<template>
  <header class="header">
    <div class="header-wrap">
      <img class="header-logo" @click="$router.push('/')" src="../assets/logo-pink.png">
      <nav class="header-nav">
        <ul>
          <li><a class="link" @click="$router.push('/')">HOME</a></li>
          <li><a class="link" @click="$router.push('/about')">ABOUT</a></li>
          <li><a class="link" @click="$router.push('/menu')">MENU</a></li>
          <li><a class="link" @click="$router.push('/sns')">SNS</a></li>
          <li><a class="link" @click="$router.push('/profile')">PROFILE</a></li>
        </ul>
      </nav>
    </div>
    <div id="hamburger" @click="hamburger()" :class="{'active':isClass}">
      <span></span>
      <span></span>
      <span></span>
    </div>
    <nav class="menu-content" :class="{'open':isClass}">
      <img class="menu-logo" src="../assets/logo_white.png">
      <ul class="menu-content_inner">
        <li><a class="link" @click="$router.push('/')">HOME</a></li>
        <li><a class="link" @click="$router.push('/about')">ABOUT</a></li>
        <li><a class="link" @click="$router.push('/menu')">MENU</a></li>
        <li><a class="link" @click="$router.push('/sns')">SNS</a></li>
        <li><a class="link" @click="$router.push('/profile')">PROFILE</a></li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isClass: false
    };
  },
  methods: {
    hamburger() {
      this.isClass = !this.isClass;
    }
  }
};
</script>
<style scoped>
.header-wrap {
  height: 90px;
  background-color: #000;
  display: flex;
  justify-content: space-between;
  align-items: center;
  z-index: 2;
}
.header-logo {
  height: 70%;
  margin: 20px 30px;
  display: flex;
}
.header-nav {
  margin-right: 30px;
  font-size: 14px;
}
.header-nav ul {
  display: flex;
}
a.header-nav li {
  padding-left: 20px;          
}
.menu-content {
  display: none;
}
@media screen and (max-width: 768px) {
  /* hamburger */
  #hamburger {
    width: 30px;
    height: 30px;
    position: absolute;
    cursor: pointer;
    top: 5px;
    right: 20px;
    transition: 0.4s;
    z-index: 100;
  }
  #hamburger span {
    position: absolute;
    left: 2px;
    display: block;
    width: 35px;
    height: 2px;
    background-color: #fac6cb;
    transition: 0.8s;
  }
  #hamburger span:nth-of-type(1) {
    top: 10px;
  }
  #hamburger span:nth-of-type(2) {
    top: 20px;
  }
  #hamburger span:nth-of-type(3) {
    top: 30px;
  }
  #hamburger.active span:nth-of-type(1) {
    top: 20px;
    transform: rotate(45deg);
  }
  #hamburger.active span:nth-of-type(2) {
    opacity: 0;
  }
  #hamburger.active span:nth-of-type(3) {
    top: 20px;
    transform: rotate(-45deg);
  }
  .menu-content {
    display: block;
    width: calc(100% - 80px);
    height: 100%;
    text-align: center;
    transition: 0.2s;
    position: fixed;
    top: 0;
    left: calc(-100% - 80px);
    background: palevioletred;
    color: #333333;
    box-shadow: 80px 0 rgba(255, 164, 164, 0.3);
    z-index: 999;
  }
  .menu-content img {
    width: 40%;
    height: 8%;
  }
  .menu-content .menu-logo {
    margin: 20px 20px;
    font-size: 2.2rem;
    color:#fff;
    font-weight: bold;
  }
  .menu-content li a {
    display: block;
    margin: 15px;
    padding: 5px;
    border-bottom: 0.5px solid palevioletred;
    color: #fff;
    text-decoration: none;
    font-size: 16px;
  }
  .menu-content.open {
    left: 0;
  }

  /* header */
  .header-nav {
    display: none;
  }
  .header-wrap {
    height: 60px;
  }
  .header-logo {
    height: 70%;
  }
}

@media screen and (max-width: 480px) {
  #hamburger {
    width: 10px;
    height: 10px;
    top: 2px;
    right: 40px;
  }
  #hamburger span {
    width: 25px;
    height: 1.5px;
  }
  #hamburger span:nth-of-type(2) {
    top: 18px;
  }
  #hamburger span:nth-of-type(3) {
    top: 26px;
  }
  .header-wrap {
    height: 50px;
  }
}
</style>