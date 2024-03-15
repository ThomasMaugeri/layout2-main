<script >
  
  import AppHeader from './components/AppHeader.vue'
  import AppNav from './components/AppNav.vue'
  
  
  

  export default {
  components:{  AppHeader,  AppNav}
  }
</script>

<template>

  <div class="container">
    <div class="left">
      <AppHeader class="header"/>
      <router-view class="page"></router-view>
    </div>
    <div class="right">

     <AppNav/>
    </div>
  
  </div>
 

  
</template>

<style lang="scss">
@use './assets/styles/general.scss' as *;

.container{
    width:100vw;
    height: 100vh;
    display: flex;
    .left{
      width: 80vw;
      .header{
        height:20vh;
      }
      .page{
        background-color: red;
        height: 80vh;
      }
    }
    .right{
      width: 20vw;
      height:100vh;
      
    }
}
  
</style>
