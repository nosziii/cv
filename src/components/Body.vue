<template>
  <div class="page-content">
    <div>
     <profile /> 
     <about />
     <skills />
     <portfoliopage />
     <experience />
     <education /> 
     <!--<reference />--> 
     <contact />
    </div>   
  </div>
</template>

<script>
import About from '../views/About.vue'
import Contact from '../views/Contact.vue'
import Education from '../views/Education.vue'
import Experience from '../views/Experience.vue'
import Portfoliopage from '../views/Portfoliopage.vue'
import Profile from '../views/Profile.vue'
//import Reference from '../views/Reference.vue'
import Skills from '../views/Skillspage.vue'

export default {
  components: { About, Skills, Portfoliopage, Experience, Education, Contact, Profile },
  name: 'Header',
  props: {
    msg: String,
  },
}
</script>

<style scoped>

</style>
