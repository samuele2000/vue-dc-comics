<template>
    <div>

        <a class="sign" href="#">SIGN-UP NOW!</a>

        <ul>
            <li>
                <h3>FOLLOW US</h3>
            </li>
            <li>
                <a><img src="../assets/img/footer-facebook.png" alt=""></a>
            </li>
            <li>
                <a><img src="../assets/img/footer-twitter.png" alt=""></a>
            </li>
            <li>
                <a><img src="../assets/img/footer-youtube.png" alt=""></a>
            </li>
            <li>
                <a><img src="../assets/img/footer-pinterest.png" alt=""></a>
            </li>
            <li>
                <a><img src="../assets/img/footer-periscope.png" alt=""></a>
            </li>
        </ul>
    </div>
</template>

<script>
    export default {
        name: 'FooterCompSocial',

    }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    @import '../style/mixin.scss';

    ul {
        @include listaOrizzontale;
        align-items: center;

        a {
            text-decoration: none;
            color: black;
            font-weight: bold;
            margin: 0 10px;
        }
        h3{
            color: $blu;
            font-weight: bolder;
            margin: 0 10px;
        }
        
    }
    

    div {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .sign{
        text-decoration: none;
        color: white;
        border: 2px solid $blu;
        padding: 10px;
        font-weight: bold;
    }
</style>