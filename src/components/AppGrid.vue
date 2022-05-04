<template>
 <div class="bg-grid">
    <ul class='row'>
      <li class='column' v-for="(elemento,index) in elementGrid" :key='index'>
        <img class='size-grid' :src="elemento.immagine" :alt="elemento.testo">
        <span class="primary-color">{{elemento.testo}}</span>
      </li>
    </ul>
 </div>
    
</template>

<script>
export default {
  name: 'AppGrid',
  data() {
    return {
        elementGrid: [
          {
            immagine: require("../assets/img/buy-comics-digital-comics.png"),
            testo: 'DIGITAL COMICS',
          },
          {
            immagine: require("../assets/img/buy-comics-merchandise.png"),
            testo: 'DC MERCHANDISE',
          },
          {
            immagine: require("../assets/img/buy-comics-subscriptions.png"),
            testo: 'SUBSCRIPTIONS',
          },
          {
            immagine: require("../assets/img/buy-comics-shop-locator.png"),
            testo: 'COMIC SHOP LOCATOR',
          },
          {
            immagine: require("../assets/img/buy-dc-power-visa.svg"),
            testo: 'DC POWER VISA',
          },
        ]
    }
  }
}
</script>


<style scoped lang="scss">
@import '../style/variables';

.bg-grid{
  background-color: $dc-color;
   @include primary-color;
   @include container;
}

.row {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  padding:70px;
  width: 100%;
  justify-content: center;
  gap: 50px;
}

.column {
  display: flex;
  flex-direction: row;
  align-self: center;
}
.size-grid{
  width: 50%;
}
span{
  align-self: center;
}
</style>