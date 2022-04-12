<template>
  <div id="app">
    <header>
      <div>
        <img src="./assets/img/dc-logo.png" alt="">
      </div>
      
      <NavComp/>
      
    </header>

  </div>
</template>

<script>
import NavComp from './components/NavComp.vue'

export default {
  name: 'App',
  components: {
    NavComp
    //HelloWorld
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

header{
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px 0;
  width: 80%;
  margin: auto;

  img{
    width: 70%;
  }
}
</style>
