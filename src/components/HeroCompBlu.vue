<template>
    <div>
        <ul>
            <li v-for="(element, index) in menuHero" :key="index">
                <img :src="element.img" alt="">
                <a href="#">{{element.name}}</a>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: 'HeroCompBlu',
        data() {
            return {
                menuHero: [{
                        name: 'DIGITAL COMICS',
                        img: require('../assets/img/buy-comics-digital-comics.png')
                    },
                    {
                        name: 'DC MERCHANDISE',
                        img: require('../assets/img/buy-comics-merchandise.png')
                    },
                    {
                        name: 'SUBSCRIPTION',
                        img: require('../assets/img/buy-comics-subscriptions.png')
                    },
                    {
                        name: 'COMIC SHOP LOCATOR',
                        img: require('../assets/img/buy-comics-shop-locator.png')
                    },
                    {
                        name: 'DC POWER VISA',
                        img: require('../assets/img/buy-dc-power-visa.svg')
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

    ul {
        @include listaOrizzontale;
        justify-content: center;
        width: 80%;
        margin: 0 auto;
        justify-content: space-between;

        li {
            display: flex;
            align-items: center;
            
        }

        img {
            width: 60px;
        }
    }

    div {
        background-color: $blu;
        padding: 40px 0;
        
        


        a {
            color: white;
            text-decoration: none;
        }
    }
</style>