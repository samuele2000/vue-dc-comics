<template>

    <ul>
        <h4>DC</h4>
        <li v-for="(element, index) in menuFooterComics" :key="index">
            <a href="`${element.url}`">{{element.name}}</a>
        </li>
    </ul>

</template>

<script>
    export default {
        name: 'FooterCompDc',
        data() {
            return {
                menuFooterComics: [{
                        name: 'Term of use',
                        url: '/Characters'
                    },
                    {
                        name: 'Privacy policy',
                        url: '/Comics'
                    },
                    {
                        name: 'Ad Choise',
                        url: '/Movies'
                    },
                    {
                        name: 'Advertising',
                        url: '/TV'
                    },
                    {
                        name: 'Jobs',
                        url: '/Games'
                    },
                    {
                        name: 'Subscription',
                        url: '/Videos'
                    },
                    {
                        name: 'Talent Workshops',
                        url: '/News'
                    },
                    {
                        name: 'CPSC Cerfificates',
                        url: '/News'
                    },
                    {
                        name: 'Ratings',
                        url: '/News'
                    },
                    {
                        name: 'shop Help',
                        url: '/News'
                    },
                    {
                        name: 'Contact Us',
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