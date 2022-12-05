<template>
   <section id="home"> 
     <div class="hero-section">
      <div class="cover-photo" :style="{ 'background-image': `url(${images.CoverImage})` }">
        <div class="cover-photo-text">
          <div class="div-spacing">
            <h1>First Aid Training Courses and Certification <span>Cape Town</span></h1>
            <ul>
              <li>Nationally Accredited &amp; Regulated</li>
              <li>Certified Instructors</li>
              <li>On- or Off-site Training</li>
              <li>Supported by Industry Leaders</li>
            </ul>
            
          </div>
        </div>
        <div class="custom-shape-divider-bottom-1669379378">
          <svg data-name="Layer 1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 120" preserveAspectRatio="none">
              <path d="M598.97 114.72L0 0 0 120 1200 120 1200 0 598.97 114.72z" class="shape-fill"></path>
          </svg>
        </div>
      </div>
      <div class="companies">
        <div class="companies-text">
          You're in good company
        </div>
        <div class="companies-images">
          <img :src="images.Northlink" alt="Northlink logo" class="northlink-logo">
          <img :src="images.Stellenbosch" alt="Stellenbosch University" class="stellenbosch-logo">
          <img :src="images.Distell" alt="Distell logo" class="distell-logo">
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import CoverImage from '@Asset/images/hero-scaled.jpg'
import Northlink from '@Asset/images/trusted/northlinklogo.png'
import Stellenbosch from '@Asset/images/trusted/SUN_logo.png'
import Distell from '@Asset/images/trusted/distell-logo-2.png'

export default {
  name: 'Hero',
  data() {
    return {
      images: {
        CoverImage,
        Northlink,
        Stellenbosch,
        Distell,
      }
    }
  },
}
</script>
<style lang="scss" scoped>
@import '../../scss/partials/variables';


.cover-photo {
  position: relative;
  margin: 65px 0 0 0;
  background-size: cover;
  padding: 200px 0;
  background-attachment: fixed;
  background-size: cover;
  background-position-y: bottom;
}

@media only screen and (max-width: 768px){
  .cover-photo{
    display: flex;
    align-items: center;
    height: calc(100vh - 65px);
    padding: 0;
    margin-top: 65px;
    background-position: right;
  }
  // .div-spacing {
  //   background: rgba(255, 255, 255, 0.4);
  //   padding: 15px 0;
  // }
}

.cover-photo h1 {
  color: #fff;
  font-size: 50px;
  justify-content: left;
  text-shadow: 2px 2px 4px #111;
  align-items: center;
  padding-left: 15%;
  padding-bottom: 15px;
  max-width: 900px;
}

@media only screen and (max-width: 525px){
  .cover-photo h1 span {
    display: block;
  }
}

@media only screen and (max-width: 768px){
  .cover-photo h1{
    font-size: 40px;
    padding: 0 20px;
  }
}

.cover-photo ul {
  display: flex;
  flex-direction: column;
  color: #fff;
  font-size: 30px;
  justify-content: left;
  text-shadow: 2px 2px 4px #111;
  padding-left: 15%;
  list-style: inside;
}

@media only screen and (max-width: 950px){
  .cover-photo h1{
    padding-left: 10%;
  }
  .cover-photo ul{
    padding-left: 10%;
  }
}

@media only screen and (max-width: 768px){
  .cover-photo h1{
    padding-left: 20px;
  }
  .cover-photo ul{
   padding: 0 20px;
   font-size: 20px;
  }
}

@media only screen and (max-width: 768px){
  .cover-photo-text{
   padding-bottom: 40px;
  }
}

.custom-shape-divider-bottom-1669379378 {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    overflow: hidden;
    line-height: 0;
}

.custom-shape-divider-bottom-1669379378 svg {
    position: relative;
    display: block;
    width: calc(100% + 1.3px);
    height: 88px;
}

.custom-shape-divider-bottom-1669379378 .shape-fill {
    fill: #FFFFFF;
}

.companies-text {
display: flex;
justify-content: center;
font-size: 30px;
padding-top: 20px;
}

@media only screen and (max-width: 900px){
  .companies-text{
    padding-bottom: 40px;
  }
}

.companies-images {
  display: flex;
  justify-content: center;
  align-items: center;
}

@media only screen and (max-width: 900px){
  .companies-images {
    flex-direction: column;
  }
}

.companies-images img {
  width: 200px;
  height: 100%;
  padding-right: 30px;
  font-weight: 700;
}
@media only screen and (max-width: 900px){
  .companies-images img {
    padding-top: 0;
    padding-right: 0;
  }
  .northlink-logo{
    padding: 40px 0;
  }
}

</style>
