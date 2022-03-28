<template>
    <div id="footer">
        <div id="footer-top">
            <div class="footer-top-content">
                <div class="footer-top-content-links">
                    <div class="col">
                        <h3>Dc Comics</h3>
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
                        <h3>Shop</h3>
                        <ul>
                            <li><a href="#"></a>Item</li>
                            <li><a href="#"></a>Item</li>
                        </ul>
                    </div>
                    <div class="col">
                        <h3>Dc</h3>
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
                        <h3>Sites</h3>
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
        <div id="footer-bottom">

        </div>
    </div>
</template>

<script>
export default {
    name: 'mainFooter'
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#footer{
    height: 50vh;
    color: white;

    #footer-top{
        height: 80%;
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        padding: 1rem 0;

        div.footer-top-content{
            @include container;
            @include d-flex;
            justify-content: space-between;
            height: 100%;

            &-links{
                width: 50%;
                @include d-flex;

                .col:nth-child(2){
                    margin: 0  2rem;
                }
                
                h3{
                    text-transform: uppercase;
                }

                ul{
                    padding: 1rem 0;

                    li{
                        font-size: .9rem;
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

    #footer-bottom{
        height: calc(100% - 80%);
        background-color: #303030;

        
    }
}

</style>