<template>
<div class="section" id="experience">
        <div class="container cc-experience">
          <div class="h4 text-center mb-4 title">Munkatapasztalat</div>
            <experience-modul/>
        </div>
      </div>
</template>

<script>
import ExperienceModul from './helpers/experience/ExperienceModul.vue'

export default {
  components: { ExperienceModul },
  name: 'Experience',

}
</script>
