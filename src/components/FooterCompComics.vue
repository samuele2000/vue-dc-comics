<template>
  <div>
      <ul>
          <h4>DC COMICS</h4>
          <li v-for="(element, index) in menuFooterComics" :key="index">
              <a href="`${element.url}`">{{element.name}}</a>
          </li>
      </ul>
  </div>
</template>

<script>

export default {
  name: 'FooterCompComics',
  data(){
      return {
          menuFooterComics: [
              {
                  name: 'Characters',
                  url: '/Characters'  
              },
              {
                  name: 'Comics',
                  url: '/Comics'   
              },
              {
                  name: 'Movies',
                  url: '/Movies'  
              },
              {
                  name: 'TV',
                  url: '/TV'  
              },
              {
                  name: 'Games',
                  url: '/Games'  
              },
              {
                  name: 'Videos',
                  url: '/Videos'  
              },
              {
                  name: 'News',
                  url: '/News'   
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
    @include listaVerticale;
}

div{
    a{
        color: grey;
        text-decoration: none;
    }
}


</style>