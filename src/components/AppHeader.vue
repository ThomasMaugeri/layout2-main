
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
    ads

  </header>
</template>

<style lang="scss" scoped>
@use '../assets/styles/general.scss' as *;
header{
  width: 100%;
  background-color: $c-header;
  height: 100%;
}
</style>
