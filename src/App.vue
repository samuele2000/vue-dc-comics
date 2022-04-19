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
        <div class="jumbotron"></div>
        <div>
          <HeroCompDark />
          <HeroCompBlu />
        </div>



      </section>
    </main>

    <footer>
      <section id="link">
        <div class="links">
          <FooterCompComics />
          <FooterCompDc />
          <FooterCompSites />
          <FooterCompShop />
          <FooterCompLogo />
        </div>

      </section>

      <section id="social">
        <FooterCompSocial />
      </section>
    </footer>
  </div>
</template>









<script>
  import NavComp from './components/NavComp.vue'
  import HeroCompDark from './components/HeroCompDark.vue'
  import HeroCompBlu from './components/HeroCompBlu.vue'
  import FooterCompComics from './components/FooterCompComics.vue'
  import FooterCompDc from './components/FooterCompDc.vue'
  import FooterCompSites from './components/FooterCompSites.vue'
  import FooterCompShop from './components/FooterCompShop.vue'
  import FooterCompSocial from './components/FooterCompSocial.vue'
  import FooterCompLogo from './components/FooterCompLogo.vue'


  export default {
    name: 'App',
    components: {
      NavComp,
      HeroCompDark,
      HeroCompBlu,
      FooterCompComics,
      FooterCompDc,
      FooterCompSites,
      FooterCompShop,
      FooterCompSocial,
      FooterCompLogo
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

  main {
    #hero {
      .jumbotron {
        height: 400px;
        background-image: url(./assets/img/jumbotron.jpg);
        background-size: cover;
      }
    }
  }




  footer {
    #link {
      background-image: url(./assets/img/footer-bg.jpg);
      padding: 20px 0;
    }

    .links {
      width: 80%;
      margin: 0 auto;
      display: flex;
      flex-wrap: wrap;
    }


    #social {
      background-color: $gray-dc;
      padding: 20px 0;
    }
  }

  .logo-dc {
    background-image: url(./assets/img/dc-logo-bg.png);
    background-size: contain;
  }
</style>