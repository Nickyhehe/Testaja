<script>
import { RouterLink, RouterView } from 'vue-router'
import Header from './views/Header.vue'
import Projects from './views/Projects.vue'
import Footer from './views/Footer.vue';

export default{
  components:{
    Header,
    Projects,
    Footer
  },

  data(){
        return{
            projects: []
        } 
            
    },

    created(){
        this.projects =[
            {
                id: 1,
                name: 'P1',
                desc: 'test aja',
                image: ("../src/assets/gerak1.gif")

            },
            {
                id: 2,
                name: 'P2',
                desc: 'test aja',
                image:  ("../src/assets/ghibli.jpg")

            },
            {
                id: 3,
                name: 'P3',
                desc: 'test aja',
                image:  ("../src/assets/ghibli.jpg")

            }
        ]

        
    }


}

</script>

<template>
  <Header/>

  <Projects :projects="projects" />

  <Footer/>
  
  <RouterView />
</template>


<style lang="sass" scoped>

</style>
