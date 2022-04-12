<template>

    <ul>
        <h4>SITES</h4>
        <li v-for="(element, index) in menuFooterComics" :key="index">
            <a href="`${element.url}`">{{element.name}}</a>
        </li>
    </ul>

</template>

<script>
    export default {
        name: 'FooterCompSites',
        data() {
            return {
                menuFooterComics: [{
                        name: 'DC',
                        url: '/Characters'
                    },
                    {
                        name: 'MAD Magazine',
                        url: '/Comics'
                    },
                    {
                        name: 'DC kids',
                        url: '/Movies'
                    },
                    {
                        name: 'DC Universe',
                        url: '/TV'
                    },
                    {
                        name: 'DC Power Visa',
                        url: '/Games'
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