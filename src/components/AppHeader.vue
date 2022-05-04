<template>
  <div>
  <div class="above-nav"></div>
  <nav>
    <img src="../assets/img/dc-logo.png" alt="">
    <ul>
      <li v-for="(item,index) in links" :key="index" :class="{'selected': item.active}">{{item.testo}}</li>
    </ul>
  </nav>
  </div>
  
</template>

<script>
export default {
  name: 'AppHeader',
  data(){
    return{
      links:[
        {
          testo:'CHARACTERS',
          active: false,
        },
        {
          testo:'COMICS',
          active: true,
        },
         {
          testo:'MOVIES',
          active: false,
        },
        {
          testo:'TV',
          active: false,
        },
        {
          testo:'GAMES',
          active: false,
        },
        {
          testo:'COLLECTIBLES',
          active: false,
        },
         {
          testo:'VIDEOS',
          active: false,
        },
        {
          testo:'FANS',
          active: false,
        },
      ]
    }
  }
}
</script>


<style scoped lang="scss">
@import '../style/variables';

.above-nav{
   height: 40px;
   background-color: $aboveNav-color;
}
nav{
  padding: 10px 0;
  @include container;
  
    img{
    width: $logo-size;
    vertical-align:middle;
    }

   ul{
    @include nav-ul;
     li{
         @include nav-li;
       }
    }
    .selected{
     border-bottom: 3px solid $dc-color;
     color: $dc-color;
    }
}
</style>
