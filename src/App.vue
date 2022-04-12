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
        <HeroComp/>
        <HeroCompBlu/>
      </section>
    </main>

    <footer>
      <FooterCompComics/>
    </footer>


  </div>
</template>

<script>
  import NavComp from './components/NavComp.vue'
  import HeroComp from './components/HeroComp.vue'
  import HeroCompBlu from './components/HeroCompBlu.vue'
  import FooterCompComics from './components/FooterCompComics.vue'

  export default {
    name: 'App',
    components: {
      NavComp,
      HeroComp,
      HeroCompBlu,
      FooterCompComics
      //HelloWorld
    }
  }
</script>

<style lang="scss">
  body{
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

    main{
      width: 80%;
      margin: auto;
      
    }
  }
</style>