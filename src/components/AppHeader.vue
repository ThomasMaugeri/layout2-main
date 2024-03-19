
<script >

export default {
    data(){
    return{
      
        
    }
  },
  methods: {
    openside() {
            if (this.sideMenuValue) {
                this.sideMenuValue = 0
            } else {
                this.sideMenuValue = 1

            }
            console.log(this.sideMenuValue)
        
        },
        infoside() {
            if (this.infomenu) {
                this.infomenu = 0
            } else {
                this.infomenu = 1
            }
        },
    
    },

  
  }
  
</script>


<template>
  <header>
    <div class="logo">

    </div>
    <h1>nome del posto</h1>

  </header>
</template>

<style lang="scss" scoped>
@use '../assets/styles/general.scss' as *;
header{
  width: 100%;
  background-color: $c-header;
  height: 100%;
  display: flex;
  padding: 2rem;
  gap:5%;
  .logo{
    background-color: black;
    width:15%;
    aspect-ratio:1 ;
    
  }
  h1{
    color: $c-text;
    text-transform: uppercase;
  }
}
</style>
