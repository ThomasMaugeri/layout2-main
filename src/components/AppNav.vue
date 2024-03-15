
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
  <div class="nav">
    <div class="link-nav">
           <router-link :to="{ name: 'home' }" class="link" >home</router-link>
           <router-link :to="{ name: 'prenotaServizio' }" class="link"  >prenota tavolo</router-link>
           <router-link :to="{ name: 'prenota' }" class="link"  >prenota asporto</router-link>
           <router-link :to="{ name: 'chi-siamo' }" class="link"  >chi siamo</router-link>
           <router-link :to="{ name: 'Contatti' }" class="link"  >contatti</router-link>
           <router-link :to="{ name: 'menu' }" class="link"  >menu</router-link>
        </div>
    <div class="info-nav">
      <div class="titoli">
        <h1>orari di apertura</h1>
        <h1>dove trovarci</h1>
      </div>
      <div class="scritti">
        <div class="left">
          <div class="top">
            <span>martedi/dom </span>
            <span>18:20/22:20</span>
          </div>
          <div class="bottom">
            <span>lunedi</span>
            <span>chiusi</span>
          </div>
          
        </div>
      </div>
      <img src="../assets/img/maps.png" alt="">
  
    </div>
</div>
</template>

<style lang="scss" scoped>
@use '../assets/styles/general.scss' as *;

.nav{
  width:100%;
  height: 100%;


  .link-nav{
    width:100%;
    height:70%;
    background-color: $c-nav;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 50px;
    align-items:center ;
    text-align: center;
     .link{
      color: white;
      font-size: 20px;
      text-transform: uppercase
     }
    
  }
  .info-nav{
    height:30%;
    background-color: green;
    padding: 20px;
    text-align: center;
    gap: 5px;
    display: flex;
    flex-direction: column;
     .titoli{
      display: flex;
      font-size: 7px;
      color: white;
      align-items: center;
      justify-content: space-between;
     }
     .scritti{
      display: flex;
      
       .left{
          display: flex;
          flex-direction: column;
          width: 50%;
          .top,.bottom{
            display: flex;
            justify-content: space-between;
          }

        }
      
     }
    img{
      max-width: 100px;
     }
  }
}
</style>
