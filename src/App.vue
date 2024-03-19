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
    height: 100vh;
    display: flex;
    overflow: hidden;
    width:100%;
    .left{
      width:100%;
      
      .header{
        height:20vh;
      }
      .page{
        background-color: red;
        overflow: auto;
      }
    }
    .right{
      
      height:100%;
      
    }
}
  
</style>
