<template>
   <section>
     <div id="intro" class="description">
       <div class="description-paragraph">
         <p>
          Every business with 10 or more employees is required by Law to have a First Aider in the workplace. One qualifies by completing a First Aid – Level 1 (CETA Accredited) course and receiving the certificate.  This course introduces basic life support that should be applied, within the workplace, until emergency services arrive.
        </p>
       </div>
     </div>
  </section>
</template>

<script>

export default {
  name: 'Intro',
}
</script>
<style lang="scss" scoped>
@import '../../scss/partials/variables';

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
    padding: 35px 10px;
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
