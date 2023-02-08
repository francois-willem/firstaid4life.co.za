<template>
   <section id="courses">
    <div class="container">
      <div class="courses">
        Courses
      </div>
      <div class="course-levels">
        <div class="course-level">
          <div class="title">First Aid - Level 1 (Occupational First Aid Training)</div>
          <div class="desc">This training is the only legally required course for workplace first aid. Regular updates ensure the course stays current with the latest amendments. This comprehensive program covers essential life-support techniques that should be implemented until emergency services arrive.
          </div>
          <div class="desc">
            On completion of the training the successful delegate will receive a Certificate, and a very detailed handbook.
          </div>
          <div class="desc">
            (SAQA Unit Standard 119567, NQF Level 1)
          </div>
        </div>
        <div class="course-level">
          <div class="title">First Aid - Level 2 (SETA Accredited)</div>
          <div class="desc">The Occupational First Aid Training - Level 2, Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur volutpat, metus sit amet egestas mollis, ante purus egestas odio, at consequat metus lectus nec est. Donec feugiat auctor fermentum. Suspendisse sodales lectus sem, non vehicula nunc vehicula eu.</div>
          <div class="desc">
            On completion of the training the successful delegate will receive a Certificate, and a very detailed handbook.
          </div>
          <div class="desc">
            (SAQA Unit Standard 120496, NQF Level 2)
          </div>
        </div>
        <div class="course-level">
          <div class="title">First Aid - Level 3 (SETA Accredited)</div>
          <div class="desc">The Occupational First Aid Training - Level 3. Mauris in porttitor erat. Nam convallis placerat purus, vitae tincidunt enim pretium a. Phasellus feugiat semper diam, quis iaculis arcu scelerisque hendrerit. Sed nisi nisi, fermentum eget magna quis, hendrerit dignissim ex. Pellentesque in tempor turpis, eget eleifend erat.</div>
          <div class="desc">
            On completion of the training the successful delegate will receive a Certificate, and a very detailed handbook.
          </div>
          <div class="desc">
            (SAQA Unit Standard 254220, NQF Level 3)
          </div>
        </div>
        <div class="course-level">
          <div class="title">Infant and Child Course</div>
          <div class="desc">The Occupational First Aid Training - Level 3. Mauris in porttitor erat. Nam convallis placerat purus, vitae tincidunt enim pretium a. Phasellus feugiat semper diam, quis iaculis arcu scelerisque hendrerit. Sed nisi nisi, fermentum eget magna quis, hendrerit dignissim ex. Pellentesque in tempor turpis, eget eleifend erat.</div>
        </div>
        <div class="course-level">
          <div class="title">Buddy Aid Course</div>
          <div class="desc">The Occupational First Aid Training - Level 3. Mauris in porttitor erat. Nam convallis placerat purus, vitae tincidunt enim pretium a. Phasellus feugiat semper diam, quis iaculis arcu scelerisque hendrerit. Sed nisi nisi, fermentum eget magna quis, hendrerit dignissim ex. Pellentesque in tempor turpis, eget eleifend erat.</div>
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
    </div>
     <div id="about-us" class="description">
       <div class="description-paragraph">
         <p>
          Our instructors are highly experienced and qualified to deliver anything from basic First Aid to advanced Prehospital Care training.
        </p>
        <p>
          We have trained Learners, Teachers, Instructors, Police, Military personnel, Business leaders and more.
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

#courses {
  padding: 35px 0 0;
}

.courses {
  display: flex;
  justify-content: center;
  font-size: 30px;
}

@media only screen and (max-width: 900px){
  .courses {
    padding-top: 20px;
  }
  #courses {
    padding: 30px 0 0;
  }
}

.course-levels {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  font-size: 25px;
  padding: 0 100px 40px;
}

@media only screen and (max-width: 900px){
  .course-levels {
    flex-direction: column;
    justify-content: left;
    padding: 0 50px;
  }
}

@media only screen and (max-width: 600px){
  .course-levels {
    flex-direction: column;
    padding: 20px 0;
  }
}

.course-level {
  padding: 20px;
  border: 1px solid #000;
  margin-top: 20px;
}

@media only screen and (max-width: 900px){
  .course-level {
    margin-top: 20px;
  }
  .course-level:first-child {
    margin-top: 0;
  }
  .course-level:last-child {
    margin-bottom: 35px;
  }
}

.course-level .title {
  color: red;
  font-family: Helvetica;
  font-size: 22px;
  font-weight: 600;
  border-bottom: 1px solid #000;
  padding-bottom: 10px;
}

.course-level .desc {
  font-size: 16px;
  font-weight: 600;
  padding-top: 15px;
}

.course-images-row-1 {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  padding: 0 15px 25px 15px;
}

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
    padding: 30px 15px 35px 15px;
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

@media only screen and (max-width: 790px){
  .description p {
    padding-left: 0;
    padding-right: 0;
  }
}

</style>
