<template>
  <main class="page-content">
    <hero></hero>
    <intro></intro>
    <courses></courses>
    <footers></footers>
  </main>
</template>

<script>
import Hero from '@Component/Home/Hero.vue'
import Intro from '@Component/Home/Intro.vue'
import Courses from '@Component/Home/Courses.vue'
import Footers from '@Component/Home/Footers.vue'

export default {
  name: 'Home',
  components: {
    Hero,
    Intro,
    Courses,
    Footers,
  },
  data() {
    return {
      
    }
  },
}
</script>
<style lang="scss" scoped>
@import '../scss/partials/variables';


</style>
