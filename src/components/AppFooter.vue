<template>
  <footer>
    <div class="bg-footer">
      <div class="row-f">
        <div class="link-footer">
          <div class="column-f">
            <ul>
              <h2>DC COMICS</h2>
              <li v-for="(element, index) in elementDcComics" :key="index">
                {{ element.testo }}
              </li>
            </ul>
          </div>
          <div class="column-f">
            <ul>
              <h2>DC</h2>
              <li v-for="(element, index) in elementDc" :key="index">
                {{ element.testo }}
              </li>
            </ul>
          </div>
          <div class="column-f">
            <ul>
              <h2>SITES</h2>
              <li v-for="(element, index) in elementSites" :key="index">
                {{ element.testo }}
              </li>
            </ul>
          </div>
          <div class="column-f">
            <ul>
              <h2>SHOP</h2>
              <li v-for="(element, index) in elementShop" :key="index">
                {{ element.testo }}
              </li>
            </ul>
          </div>
        </div>
        <div class="img-footer">
          <img src="../assets/img/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </div>
    <div class="black">
      <div class='container-footer'>
        <button>SIGN-UP NOW!</button>
        <ul>
          <li><a href="">FOLLOW US</a></li>
          <li><img src="../assets/img/footer-facebook.png" alt=""></li>
          <li><img src="../assets/img/footer-twitter.png" alt=""></li>
          <li><img src="../assets/img/footer-youtube.png" alt=""></li>
          <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
          <li><img src="../assets/img/footer-periscope.png" alt=""></li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
  data() {
    return {
      elementDcComics: [
        {
          testo: "Characters",
          link: "",
        },
        {
          testo: "Comics",
          link: "",
        },
        {
          testo: "Movies",
          link: "",
        },
        {
          testo: "TV",
          link: "",
        },
        {
          testo: "Games",
          link: "",
        },
        {
          testo: "Videos",
          link: "",
        },
        {
          testo: "News",
          link: "",
        },
      ],

      elementDc: [
        {
          testo: "Terms Of Use",
          link: "",
        },
        {
          testo: "Privacy policy(New)",
          link: "",
        },
        {
          testo: "Ad Choices",
          link: "",
        },
        {
          testo: "Advertising",
          link: "",
        },
        {
          testo: "Jobs",
          link: "",
        },
        {
          testo: "Subscriptions",
          link: "",
        },
        {
          testo: "Talent Workshops",
          link: "",
        },
        {
          testo: "CPSC Certificates",
          link: "",
        },
        {
          testo: "Rating",
          link: "",
        },
        {
          testo: "Shop Help",
          link: "",
        },
        {
          testo: "Contact Us",
          link: "",
        },
      ],
      elementSites: [
        {
          testo: "DC",
          link: "",
        },
        {
          testo: "MAD Magazine",
          link: "",
        },
        {
          testo: "DC Kids",
          link: "",
        },
        {
          testo: "DC Universe",
          link: "",
        },
        {
          testo: "DC Power Visa",
          link: "",
        },
      ],
      elementShop: [
        {
          testo: "Shop DC",
          link: "",
        },
        {
          testo: "Shop DC Collectibles",
          link: "",
        },
      ],
    };
  },
};
</script>


<style scoped lang="scss">
@import "../style/variables";

.bg-footer {
  @include primary-color;
  @include container;
  background-image: url(../assets/img/footer-bg.jpg);
  width: 100%;
}
.row-f {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  padding: 50px 0px 3px;
  width: 100%;
  gap: 0px;
}
.column-f {
  display: inline-block;
  width: 33%;
  line-height: 27px;
}
li {
  list-style: none;
  color: $footer-text;
}
.link-footer {
  display: flex;
  flex-wrap: inherit;
}

.img-footer {
  display: inline-block;
  width: 48%;
  img {
    width: 90%;
  }
}

.black {
  background-color: #2A2A2A;
  padding: 30px
}
.container-footer{
  @include container;
  
  button{
    border: 1px solid $dc-color;
    background-color:#2A2A2A;
    @include primary-color;
    padding: 10px 14px;
  }
  
  ul{
    @include nav-ul;
    padding: 0;
     li{
         @include nav-li;
         a{
           text-decoration: none;
           color: $dc-color;
           font-size: 16px;
           position: relative;
           bottom: 11px;
         }
       }
    }
}

</style>