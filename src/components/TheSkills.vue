<script>
import SkillCard from './SkillCard.vue'
export default{
  components:{
    SkillCard
  },
    data(){
        return{
            skills:[
                {
                    id:1,
                    title:'JavaScript',
                    'desc':`Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
            'percent':'10'
                },
                    {
                    id:2,
                    title:'html',
                    'desc':`Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
            'percent':'20'
                },
                    {
                    id:3,
                    title:'css',
                    'desc':`Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
            'percent':'30'
                },

            ]
        }
    }
}
</script>

<template>
  <div class="bg-dark">
    <div class="container">
      <h3 class="text-warning skill-header">The SKILLS</h3>
      <!-- skill 1 -->
        <SkillCard v-for="skill in skills" :key="skill.id" :title="skill.title" :desc="skill.desc" :percent="skill.percent" />
      <!-- end of skill one -->
    </div>
  </div>
</template>

<style scoped>
.skill-header {
  text-align: center;
}
</style>
