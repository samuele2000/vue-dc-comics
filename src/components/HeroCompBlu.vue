<template>
  <div>
      <ul>
          <li v-for="(element, index) in menuHero" :key="index">
              <img src="`../assets/img/element.img`" alt="">
              <a href="#">{{element.name}}</a>
          </li>
      </ul>
  </div>
</template>

<script>

export default {
  name: 'HeroCompBlu',
  data(){
      return {
          menuHero: [
              {
                  name: 'DIGITAL COMICS',
                  img: 'buy-comics-digital-comics.png'  
              },
              {
                  name: 'DC MERCHANDISE',
                  img: 'buy-comics-merchandise.png'  
              },
              {
                  name: 'SUBSCRIPTION',
                  img: 'buy-comics-subscriptions.png'  
              },
              {
                  name: 'COMIC SHOP LOCATOR',
                  img: 'buy-comics-shop-locator.png'  
              },
              {
                  name: 'DC POWER VISA',
                  img: 'buy-dc-power-visa.png'  
              },
          ]
      }
  }    
  }

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../style/variabili.scss';
@import '../style/mixin.scss';

ul{
    @include listaOrizzontale;
    justify-content: center;
}

div{
    background-color: $blu;
    padding: 40px 0;
    a{
        color: white;
        text-decoration: none;
        margin: 0 20px;
    }
}


</style>