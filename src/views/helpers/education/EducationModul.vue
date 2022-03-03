<template>
        <div>
         <div class="card" v-for="(card, index) in education" :key="`${index}-${card.educationName}`">
            <div class="row">
              <div class="col-md-3 bg-primary" data-aos="fade-right" data-aos-offset="50" data-aos-duration="500">
                <div class="card-body cc-education-header">
                  <p>{{card.date}}</p>
                  <div class="h5">{{card.educationName}}</div>
                </div>
              </div>
              <div class="col-md-9" data-aos="fade-left" data-aos-offset="50" data-aos-duration="500">
                <div class="card-body">
                  <div class="h5">{{card.education}}</div>
                  <p>{{card.pbody}}</p>
                  <p>{{card.helpy}}<a :href="card.link">{{card.linkName}}</a></p>
                <div v-for="(el, i) in card.liBody" :key="`${i}-libody`">
                    <li>{{el}}</li>
                </div>
                </div>
              </div>
            </div>
          </div>
        </div>
</template>

<script>

const educationData = require("./educationData")

export default {
  name: 'EducationModul',

  created(){
      console.log("===data", educationData.default)
      this.education = educationData.default
    },

  data (){
    return {
        education: []
    }
   }
        
}
</script>
