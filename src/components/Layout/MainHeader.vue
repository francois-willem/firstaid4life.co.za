<template>
  <header>
    <nav class="desktop">
      <div class="wrapper1">
        <div class="logo">
          <a href="#home">
             <img :src="images.Logo" alt="logo">
          </a>
        </div>
        <div class="wrapper-menu">
          <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about-us">About Us</a></li>
            <li><a href="#courses">Courses</a></li>
            <li><a href="#contact-us">Contact Us</a></li>
          </ul>
        </div>
      </div>
    </nav>

    <nav class="mobile">
      <div class="wrapper2">
        <div class="logo">
          <img :src="images.Logo" alt="full-logo">
        </div>

        <a href="#contact-us">Contact Us</a>
      </div>      
    </nav>

  </header>
</template>

<script>
import Logo from '@Asset/images/firstaid4lifetext.png'

export default {
  name: 'MainHeader',
  components: {
  },
  data() {
    return {
      images: {
        Logo
      },
      isMobile: true,
      isDesktop: false,
      isHeaderHeightDoubleLineForTopBanner: false
    }
  },
  methods: {
    setDeviceVariables() {
      if (document.documentElement.clientWidth < 1024) {
        this.isMobile = true
        this.isDesktop = false
      } else {
        this.isMobile = false
        this.isDesktop = true
      }
    },
  },
}
</script>

<style lang="scss" scoped>
@import '../../scss/partials/variables';
$background-color: $dark-color;

.wrapper1 {
  display: flex;
  justify-content: space-between;
  background-color: #ffffff;
  width: 100%;
  padding: 0 15px;
  margin: 0 auto;
}

.wrapper-menu {
  
}

.logo {
  display: flex;
  align-items: center;
}

.logo img {
  height: 40px;
}

// .logotext {
//   display: flex;
//   align-items: center;
//   font-size: 25px;
//   color: #272361;
//   padding-left: 20px;
// }

nav.mobile {
  display: none;
}

@media only screen and (max-width: 768px){
  nav.desktop {
    display: none;
  }

  nav.mobile {
    display: block;
  }
}



.wrapper2 {
  display: flex;
  justify-content: space-between;
  padding: 15px 15px;
} 

header {
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  width: 100%;
  height: 65px;
  z-index: 999;
}

@media only screen and (max-width: 768px){
  header {
    height: 65px;
  }
}

nav {
  display: flex;
  justify-content: center;
  width: 100%;
  height: 65px;
  background-color: #ffffff;
}

@media only screen and (max-width: 768px){
  nav {
    height: 65px;
  }
}

body header nav ul {
  display: flex;
  margin-left: 0;
  justify-content: center;
}

body header nav ul li {
  display: flex;
  align-items: center;
  list-style: none;
  display: inline-block;
  line-height: 65px;
}

body header nav ul li a {
  display: block;
  text-decoration: none;
  font-size: 22px;
  color: #000000;
  padding: 0 40px 0 0;
}

@media only screen and (max-width: 800px){
  body header nav ul li a{
    font-size: 20px;
  }
}

.wrapper2 a {
  display: block;
  text-decoration: none;
  font-size: 22px;
  color: #000000;
  align-self: center;
}

@media only screen and (max-width: 800px){
  .wrapper2 a {
    font-size: 20px;
  }
}
</style>
