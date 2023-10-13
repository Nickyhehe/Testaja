<template>
    
        
    <div class="Project" @mouseenter="showPopup=true" @mouseleave="showPopup=false">
        <img :src="Project.image" :alt="Project.image"/>
        <h1 >{{Project.name}}</h1>
        <p>{{Project.desc}}</p>
            
        <!-- <div class="popup" v-if="showPopup">
        <h1 >{{Project.name}}</h1>
        <p>{{Project.desc}}</p>
        </div> -->
    </div>

      
</template>

<script>

export default{
    
    name: 'Project',
    props:{
        Project : Object
    },
    data(){
      return{

        showPopup : false
      }
    },
    methods:{
    
    }
  

}
</script>

<style lang="scss">


.Project{
  padding: 3vw;
  text-align: center;
  border: 1px solid #ddd;
  border-radius: 25px;
  align-items: center;
  position: relative;
  

  h1{
    font-size: 4vw;
  }
  p{
    font-size: 3vw;
  }


  img{
    width: 100vw;
    height: 30vh;
    max-width: 100%;
    border-radius: 25px;
  }

  

}



</style>