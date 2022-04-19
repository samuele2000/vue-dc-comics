<template>
    <div>
        <ul>
            <li>
                <img :src="src" alt="">
                <a href="#">{{nome}}</a>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: 'ComicsComp',
        props: {
            src: String,
            nome: String
        }
    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    div{
        width: calc(100% / 6);
    }
    ul{
        margin: 0 10px 10px 10px;
        padding: 0;
    }
    li{
        list-style-type: none;
    }
    a{
        text-decoration: none;
        font-weight: bold;
        color: white;
        text-transform: uppercase;
    }
    img{
        width: 100%;
    }
</style>