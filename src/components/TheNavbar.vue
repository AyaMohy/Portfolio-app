<script>
import TheSkills from './TheSkills.vue';
import TheProjects from './TheProjects.vue';
import Contact from './Contact.vue'

export default{
  components:{
    TheSkills,
    TheProjects,
    Contact
  },
  data(){
    return{
      currentTab:'TheSkills'
    }
  }
}
</script>
<template>
    <div>
          <nav class="navbar navbar-expand-lg bg-dark navbar-dark">
      <div class="container">
        <a class="navbar-brand"   @click.prevent="$emit('change-current-tab', 'TheSkills')" role="button">Portfolio</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav mb-2 mb-lg-0 ms-auto">
            <li class="nav-item">
              <a class="nav-link " role="button" aria-current="page"
               @click.prevent="$emit('change-current-tab', 'TheProjects')"
             
                >Projects</a
              >
            </li>
            <li class="nav-item">
              <a class="nav-link" role="button" @click.prevent="$emit('change-current-tab', 'Contact')">Contact</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>


 
    </div>
</template>

<style scoped>
  a{
    display: inline-block;
    transition:  all 2s;
  }
a:hover{
  border-bottom: 1px solid white;
}

</style>