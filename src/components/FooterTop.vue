<template>
    <div id="footer-top">
        <div class="footer-top-content">
            <div class="footer-top-content-links">
                <div class="col">
                    <h4>Dc Comics</h4>
                    <ul>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                    </ul>
                    <h4>Shop</h4>
                    <ul>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                    </ul>
                </div>
                <div class="col">
                    <h4>Dc</h4>
                    <ul>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                    </ul>
                </div>
                <div class="col">
                    <h4>Sites</h4>
                    <ul>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                        <li><a href="#"></a>Item</li>
                    </ul>
                </div>
            </div>
            <div class="footer-top-bg">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterTop'
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#footer-top{
    height: 80%;
    background-image: url(../assets/img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;

    div.footer-top-content{
        @include container;
        @include d-flex;
        justify-content: space-between;
        height: 100%;

        &-links{
            width: 50%;
            padding: 1rem 0;
            @include d-flex;

            .col:nth-child(2){
                margin: 0  2rem;
            }
            
            h4{
                text-transform: uppercase;
            }

            ul{
                padding: 1rem 0;

                li{
                    font-size: .6rem;
                    color: #7f7f7f;
                }
            }

            
        }

        div.footer-top-bg{
            width: 40%;
            height: 100%;
            background-image: url(../assets/img/dc-logo-bg.png);
            background-repeat: no-repeat;
            background-size: cover;
            background-position: center;
        }
    }
}



</style>