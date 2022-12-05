<template>
   <section id="courses">
    <div class="container">
      <div class="courses">
        Courses
      </div>
      <div class="course-levels">
        <div class="course-level">
          Level 1
        </div>
        <div class="course-level">
          Level 2
        </div>
        <div class="course-level">
          Level 3
        </div>
      </div>
      <div class="course-images-row-1">
        <div class="course-image-container">
          <img :src="images.Image1" alt="">
        </div>
        <div class="course-image-container">
          <img :src="images.Image2" alt="">
        </div>
        <div class="course-image-container">
          <img :src="images.Image3" alt="">
        </div>
        <div class="course-image-container">
          <img :src="images.Image4" alt="">
        </div>
        <div class="course-image-container">
          <img :src="images.Image5" alt="">
        </div>
        <div class="course-image-container">
          <img :src="images.Image6" alt="">
        </div>
      </div>
      <!-- <div class="course-images-row-2">
        <div class="course-image-container">
          <img :src="images.Image4" alt="">
        </div>
        <div class="course-image-container">
          <img :src="images.Image5" alt="">
        </div>
        <div class="course-image-container">
          <img :src="images.Image6" alt="">
        </div>
      </div> -->
    </div>
     <div id="about-us" class="description">
       <div class="description-paragraph">
         <p>
          Our instructors are highly experienced and qualified to deliver anything from basic First Aid to advanced Prehospital Care training.
        </p>
        <p>
          We have trained Teachers, Instructors, Paramedics, Nurses, Doctors, Police, Military personel, Business leaders and more.
        </p>
        <p>
          We aim to deliver the best training on the market, not neccesarily the cheapest, through high standards and with quality resources.
        </p>
       </div>
     </div>
  </section>
</template>

<script>
import Image1 from '@Asset/images/scaled/course-img-1.jpg'
import Image2 from '@Asset/images/scaled/course-img-2.jpg'
import Image3 from '@Asset/images/scaled/course-img-3.jpg'
import Image4 from '@Asset/images/scaled/course-img-4.jpg'
import Image5 from '@Asset/images/scaled/course-img-5.jpg'
import Image6 from '@Asset/images/scaled/course-img-6.jpg'

export default {
  name: 'Courses',
  data() {
    return {
      images: {
        Image1,
        Image2,
        Image3,
        Image4,
        Image5,
        Image6,
      }
    }
  },
}
</script>
<style lang="scss" scoped>
@import '../../scss/partials/variables';

.courses {
  display: flex;
  justify-content: center;
  font-size: 30px;
  padding-top: 20px;
  text-shadow: 1px 2px 5px #111;
}

.course-levels {
  display: flex;
  justify-content: space-around;
  align-items: center;
  font-size: 25px;
  padding: 20px 100px;
}

@media only screen and (max-width: 900px){
  .course-levels {
    flex-direction: column;
  }
}

.course-images-row-1 {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  padding: 0 15px 20px 15px;
}

// .course-images-row-1 :last-child {
//   padding-right: 0;
// }

// .course-images-row-2 {
//   display: flex;
//   flex-wrap: wrap;
//   justify-content: space-around;
//   padding: 0 15px 20px 15px;
// }

// .course-images-row-2 :last-child {
//   padding-right: 0;
// }

.course-image-container {
  display: flex;
  padding: 0 10px 10px 0;
}

.course-image-container img {
  width: 350px;
}

@media only screen and (max-width: 759px){
  .course-image-container {
    padding-right: 0;
  }
}

.description {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  background-color: #0E5290;
  padding: 20px 0;
  width: 100%;
}

@media only screen and (max-width: 759px){
  .description {
    padding: 0 20px;
  }
}

.description-paragraph {
  max-width: 700px;
  
}

.description p {
  padding: 10px;
  color: #fff;
  font-size: 20px;
}

</style>
