<template>
 <div class="section">
        <div class="container cc-education">
          <div class="h4 text-center mb-4 title">Education</div>
         <education-modul/>
        </div>
      </div>
</template>

<script>
import EducationModul from './helpers/education/EducationModul'

export default {
  components: { EducationModul },
  name: 'Education',

}
</script>
