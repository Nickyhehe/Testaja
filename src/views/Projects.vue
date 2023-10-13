<script>
import Project from './Project.vue';

export default{
    name:'Projects',

    components:{
        Project,
    },
    props:{
        projects : Array

    }

}

</script>

<template>

    <div class="project-container">
        <div v-for="project in projects" :key="project.id">
            <Project :Project="project" />
        </div>
    </div>
 

</template>

<style lang="scss" scoped>
.project-container{
    padding: 7vw;
    display: grid;
    grid-template-columns: repeat( 3, 1fr);
    gap: 4vw;

}

@media (max-width: 768px) {
    .project-container {
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); 
    }
  }
  
  @media (max-width: 480px) {
    .project-container {
      grid-template-columns: 1fr; 
    }
  }
    

</style>