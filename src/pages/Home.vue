
<script >
  
  export default {
    data(){
    return{
       
    }
  },
  methods: {
   
    },

  
  }
</script>


<template>
<div class="main">
  <div class="carosello-img">
    <img src="../assets/img/bigimage.png" alt="">
  </div>
  <div class="text">
    <h1>Titolo Paragrafo</h1>
    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ratione quis reiciendis, accusantium atque incidunt nobis est commodi possimus beatae blanditiis assumenda, illum aut distinctio tempore debitis nostrum ullam voluptatem repellendus.</p>
    <a href=""><span>prenota</span></a>
  </div>
</div>
  
</template>

<style lang="scss" scoped>
@use '../assets/styles/general.scss' as *;

.main{
  display: flex;
 .carosello-img{
  width:60%;
  img{
    max-width:100%;
    height:80%;
  }
 }
  .text{
    width:20%;
    align-items:flex-start;
    display: flex;
    flex-direction: column;
    gap: 3%;
    margin:5%;
    h1{
      margin-top:20%;
      text-transform: uppercase;
      font-size:20px;
      
    }
    p{
      margin-bottom:20%;
      font-size:20px;
    }
    a{
      background-color: white;
      width:50%;
      height:5%;
      text-align: center;
      display: flex;
      justify-content: center;
      align-items: center;
      text-transform: uppercase;
      }
  }
} 




</style>
