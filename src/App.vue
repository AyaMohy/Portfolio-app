<script>
import TheNavbar from './components/TheNavbar.vue'
import TheBanner from './components/TheBanner.vue'
import TheSkills from './components/TheSkills.vue';
import Contact from './components/Contact.vue';
import TheProjects from './components/TheProjects.vue';
export default {
  components:{
    TheNavbar,
    TheBanner,
    TheSkills,
    Contact,
    TheProjects
  },
  data(){
    return{
      currentTab:'TheSkills'
    }
  },
  methods:{
    currentTabBehaviour(tab){
      this.currentTab=tab
    }
  }
};
</script>

<template>
  <div>
  <TheNavbar @change-current-tab='currentTabBehaviour'/>
  <TheBanner/>
  <component :is="currentTab"></component>
  </div>
</template>

<style></style>
