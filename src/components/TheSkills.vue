<script>
import SkillCard from './SkillCard.vue'
export default {
  components: {
    SkillCard
  },
  data() {
    return {
      skills: [
      {
          id: 1,
          title: 'html',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '95'
        },
        {
          id: 2,
          title: 'Bootstrap',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '95'
        },
        {
          id: 5,
          title: 'JavaScript and Es6',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '90'
        },
        {
          id: 6,
          title: 'css',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '90'
        },
        {
          id: 15,
          title: 'C Language',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '90'
        },
      {
          id: 3,
          title: 'Vue JS',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '80'
        },
        {
          id: 4,
          title: 'React JS',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '80'
        },
  
      
        {
          id: 8,
          title: 'Vue Router ',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '80'
        },
        {
          id: 9,
          title: 'React Router Dom',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '80'
        },
        {
          id: 10,
          title: 'Pinia state management',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '80'
        },
        {
          id: 10,
          title: 'Redux Toolkit',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '80'
        },
        {
          id: 11,
          title: 'Material Ui',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '80'
        },
        {
          id: 14,
          title: 'Git',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '80'
        },
        {
          id: 20,
          title: 'Firebase',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '80'
        },
        {
          id: 7,
          title: 'Sass',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '70'
        },
        {
          id: 10,
          title: 'VeeValidate',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '70'
        },
     
        {
          id: 12,
          title: 'Socket Io',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '70'
        },
      
        {
          id: 13,
          title: 'Socket Io',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '70'
        },
        {
          id: 18,
          title: 'My SQL DB',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '70'
        },
        {
          id: 13,
          title: 'Nuxt JS',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '60'
        },
        {
          id: 17,
          title: 'Laravel',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '60'
        },
        {
          id: 16,
          title: 'Node JS',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '50'
        },
      
       
        {
          id: 19,
          title: 'Mongo DB',
          'desc': `Some placeholder content for the collapse component. This panel is
            hidden by default but revealed when the user activates the relevant
            trigger.`,
          'percent': '50'
        },
       

      ]
    }
  }
}
</script>

<template>
  <div class="bg-dark">
    <div class="container skill-wrapper">
      <h3 class="text-warning skill-header">The SKILLS</h3>
      <!-- skill 1 -->
      <SkillCard v-for="skill in skills" :key="skill.id" :title="skill.title" :desc="skill.desc"
        :percent="skill.percent" />
      <!-- end of skill one -->
    </div>
  </div>
</template>

<style scoped>
  .skill-wrapper{
    padding-bottom: 100px;
  }
.skill-header {
  text-align: center;
}
</style>
