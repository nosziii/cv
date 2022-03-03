<template>
        <div>
          <div class="card" v-for="(card, index) in experience" :key="`${index}-${card.companyName}`">
            <div class="row">
              <div class="col-md-3 bg-primary" data-aos="fade-right" data-aos-offset="50" data-aos-duration="500">
                <div class="card-body cc-experience-header">
                  <p>{{card.date}}</p>
                  <div class="h6">{{card.companyName}}</div>
                </div>
              </div>
              <div class="col-md-9" data-aos="fade-left" data-aos-offset="50" data-aos-duration="500">
                <div class="card-body">
                  <div class="h5">{{card.experient}}</div>
                  <div v-for="(p_up, i) in card.pheader" :key="`${i}-pheader`">
                    <p >{{p_up}}</p>
                  </div>
                <div v-for="(libody, i) in card.libody" :key="`${i}-li`">
                    <li>{{libody}}</li>
                </div>
                    <div v-for="(p_down, i) in card.pfooter" :key="`${i}-pfooter`">
                    <p >{{p_down}}</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
</template>

<script>

const experienceData = require("./experienceData")

export default {
  name: 'ExperienceModul',

  created(){
      this.experience = experienceData.default
    },

  data (){
    return {
        experience: []
    }
   }
        
}
</script>
