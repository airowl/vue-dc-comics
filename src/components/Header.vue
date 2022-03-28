<template>
    <div id="header">
        <div class="main-logo">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
        </div>
        <nav class="header-nav">
            <ul>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">Tv</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Collectibles</a></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">Fans</a></li>
                <li><a href="#">News</a></li>
                <li><a href="#">Shop</a></li>
            </ul>
        </nav>
    </div>
</template>

<script>
export default {
    name: 'mainHeader'
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#header{
    @include container;
    @include d-flex;
    justify-content: space-between;
    align-items: center;
    height: 15vh;
    border: 1px solid red;

    nav.header-nav{
        
        height: 100%;

        ul{
            height: 100%;
            @include d-flex;
            justify-content: center;

            li{
                list-style-type: none;
                margin-left: 2rem;
                height: 100%;
                @include d-flex;
                align-items: center;
                border-bottom: 4px solid transparent;

                &.active,
                &:hover{
                    border-bottom: 4px solid $secondaryColor;
                }

                a{
                    text-decoration: none;
                    color: $fontColor;
                    text-transform: uppercase;
                    font-size: .8rem;
                }
            }
        }
    }

}

</style>
