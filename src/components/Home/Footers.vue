<template>
  <section id="contact-us">
     <div class="footer-container">
       <div class="container">
        <div class="footer-column">
          <p>
            Contact Us
          </p>
          <div class="item-container">Cell: 084 413 5051</div>
          <div class="item-container">Whatsapp: 084 413 5051</div>
          <div class="item-container">Email: ciske@firstaid4life.co.za</div>
        </div>
        <div class="footer-column">
          <p>
            Business Hours
          </p>
          <div class="item-container">Monday - Friday 9am - 5pm</div>
          <div class="item-container">Saturday - Closed for training</div>
          <div class="item-container">Sunday - Closed for training</div>
        </div>
        <div class="footer-column">
          <p>
            Address
          </p>
          <div class="item-container">Plattekloof 1,</div>
          <div class="item-container">Northern Suburbs, </div>
          <div class="item-container">Cape Town</div>
        </div>
      </div>
     </div>
     <div class="divider">

     </div>
     <div class="copyright-container">
       Copyright © 1997–2022 First Aid 4 Life. All rights reserved.
     </div>
  </section>
</template>

<script>

export default {
  name: 'Footers',
  data() {
    return {
      images: {
        
      }
    }
  },
}
</script>
<style lang="scss" scoped>
@import '../../scss/partials/variables';

.footer-container {
  display: flex;
  background-color: #094072;
  justify-content: center;
  padding: 20px 0;
}

.footer-container:last-child {
  padding-right: 0;
}

.container {
  display: flex;
  justify-content: center;
}

@media only screen and (max-width: 790px){
  .container {
    flex-direction: column;
  }
}


.footer-column {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  padding: 0 15px 20px 15px;
  flex: 1;
}

@media only screen and (max-width: 790px){
  .footer-column {
    padding: 0 0 20px 0;
  }
}

.footer-column p {
  color: #fff;
  font-size: 25px;
  padding-bottom: 15px;
}

.item-container {
  color: #fff;
  padding-bottom: 7px;
  font-size: 18px;
}

.divider {
  background-color: #0f0f0f ;
  height: 1.5px;
  width: 100%;
}

.copyright-container {
  display: flex;
  justify-content: center;
  background-color: #094072;
  color: #fff;
  font-size: 14px;
  padding: 15px 0;
}

</style>
