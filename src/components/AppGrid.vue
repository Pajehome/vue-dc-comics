<template>
  <div>
    <ul>
      <li v-for="(elemento,index) in elementGrid" :key='index'>
        <img :src="elemento.immagine" :alt="elemento.testo">
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

</style>