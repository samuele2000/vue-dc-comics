<template>
  <div id="app">
    <header>
      <div>
        <img src="./assets/img/dc-logo.png" alt="">
      </div>
      <NavComp />
    </header>

    <main>
      <!-- hero -->
      <section id="hero">
        <HeroComp />
        <HeroCompBlu />
      </section>
    </main>

    <footer>
      <section id="link">
        <div>
          <FooterCompComics />
          <FooterCompDc />
          <FooterCompSites />
          <FooterCompShop />
        </div>
      </section>
     
      <section id="social">
        <FooterCompSocial/>
      </section>



    </footer>





  </div>
</template>

<script>
  import NavComp from './components/NavComp.vue'
  import HeroComp from './components/HeroComp.vue'
  import HeroCompBlu from './components/HeroCompBlu.vue'
  import FooterCompComics from './components/FooterCompComics.vue'
  import FooterCompDc from './components/FooterCompDc.vue'
  import FooterCompSites from './components/FooterCompSites.vue'
  import FooterCompShop from './components/FooterCompShop.vue'
  import FooterCompSocial from './components/FooterCompSocial.vue'


  export default {
    name: 'App',
    components: {
      NavComp,
      HeroComp,
      HeroCompBlu,
      FooterCompComics,
      FooterCompDc,
      FooterCompSites,
      FooterCompShop,
      FooterCompSocial
    }
  }
</script>

<style lang="scss">
@import './style/variabili.scss';

  body {
    margin: 0;
  }

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    //text-align: center;

  }

  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0;
    width: 80%;
    margin: auto;

    img {
      width: 70%;
    }
  }

 

  footer {
    #link {
      background-image: url(./assets/img/footer-bg.jpg);
      padding: 20px 0;
      display: flex;
    }

    div {
      width: 80%;
      margin: auto;
      display: flex;
      flex-wrap: wrap;
    }

    #social{
      background-color: $gray-dc;
      padding: 20px 0;
    }

  }
</style>