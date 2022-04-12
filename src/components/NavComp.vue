<template>
  <div>
      <ul>
          <li>
              <a href="/characters">CHARACTERS</a>
          </li>
          <li >
              <a class="select" href="/characters">COMICS</a>
          </li>
          <li>
              <a href="/characters">MOVIES</a>
          </li>
          <li>
              <a href="/characters">TV</a>
          </li>
          <li>
              <a href="/characters">GAMES</a>
          </li>
          <li>
              <a href="/characters">COLLECTIBLES</a>
          </li>
          <li>
              <a href="/characters">VIDEOS</a>
          </li>
          <li>
              <a href="/characters">FANS</a>
          </li>
          <li>
              <a href="/characters">NEWS</a>
          </li>
          <li>
              <a href="/characters">SHOP</a>
          </li>
      </ul>
  </div>
</template>

<script>

export default {
  name: 'NavComp',
       
  }

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../style/mixin.scss';

ul{
    @include listaOrizzontale;
    a{
        text-decoration: none;
        color: black;
        font-weight: bold;
        margin: 0 10px;
    }
}

.select{
    color: $blu;
    border-bottom: 5px solid $blu;
}

</style>