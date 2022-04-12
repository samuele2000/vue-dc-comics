<template>
    <ul>
        <h4>SHOP</h4>
        <li v-for="(element, index) in menuFooterComics" :key="index">
            <a href="`${element.url}`">{{element.name}}</a>
        </li>
    </ul>

</template>

<script>
    export default {
        name: 'FooterCompShop',
        data() {
            return {
                menuFooterComics: [{
                        name: 'Shop DC',
                        url: '/Characters'
                    },
                    {
                        name: 'Shop DC Collectibles',
                        url: '/Comics'
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
        @include listaVerticale;
        h4{
            color: white;
        }
    }


    a {
        color: grey;
        text-decoration: none;
    }
</style>