
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
    <div class="top-nav">
      <router-link :to="{ name: 'home' }" class="link" >home</router-link>
      <router-link :to="{ name: 'menu' }" class="link"  >menu</router-link>
      <router-link :to="{ name: 'prenota' }" class="link"  >prenota asporto</router-link>
      <router-link :to="{ name: 'prenotaServizio' }" class="link"  >prenota tavolo</router-link>
      <router-link :to="{ name: 'chi-siamo' }" class="link"  >chi siamo</router-link>
      <router-link :to="{ name: 'Contatti' }" class="link"  >contatti</router-link>
    </div>
    <div class="bottom-nav">
      <div class="top-bottom-nav">
        <div class="left-info">
          <h4>orari di apertura</h4>
          <div class="left-time">
            <span>martedi/dom</span>
            <span>lunedi</span>
            <span>18:30-22:30</span>
            <span>chiusi</span>
          </div>
        </div>
        <div class="right-info">
          <h4>dove trovarci</h4>
          <span>Lorem ipsum dolor sit amet consectetur </span>
        </div>
      </div>
      <img src="../assets/img/maps.png" alt="">
    </div>
 </div>
</template>

<style lang="scss" scoped>
@use '../assets/styles/general.scss' as *;
.nav{
  height:100%;
  .top-nav{
    background-color:$c-nav;
    display: flex;
    height: 70%;
    flex-direction: column;
    justify-content: space-between;
    padding:15%;
    align-items: center;
    text-transform: uppercase;
    .link{
      color:$c-text;

    }
  }
  .bottom-nav{
    padding:2rem;
    background-color:$c-header ;
    height:30%;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    width:clamp(220px,30vw,350px);
    .top-bottom-nav{
      display: flex;
      justify-content: space-between;
      
    }
    .left-info,.right-info{
      display: flex;
      flex-direction: column;
      color: $c-text;
      gap:5%;
      h4{
        margin-bottom:5%;
        text-transform: uppercase;
        white-space:nowrap;
        font-size:clamp(12px,2vw,16px);
      }
    }
    img{
      width:100%;
      aspect-ratio: 2;
      border: 3px solid $c-text;
      border-radius: 10px;
    }
  }
}

</style>
