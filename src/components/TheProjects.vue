<script>
import projects from '../../projects.json';
import ProjectCardVue from './ProjectCard.vue';
export default {
  data() {
    return {
      projects
    }
  },
  components: {
    ProjectCardVue
  }
}
</script>

<template >
  <div class="bg-dark py-3">

    <div class="container">


      <div class="d-flex justify-content-between  flex-wrap">
        <ProjectCardVue v-for="(project, $index) in projects" :key="$index" :title="project.title"
          :description="project.desc" :links="project.links"/>

      </div>
    </div>
  </div>
</template>




