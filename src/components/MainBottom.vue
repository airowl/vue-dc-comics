<template>
    <div id="main-bottom">
        <div class="container">
            <ul>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        <p>Digital Comics</p>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        <p>Dc merchandise</p>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        <p>Subsription</p>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                        <p>Comic Shop Locator</p>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                        <p>Dc Power Visa</p>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'mainBottom',
    data: function() {
        return {
            //mainBottomLinks: [
            //    {
            //        text: 'Digital Comics',
            //        url: '#',
            //        image: '../assets/img/buy-comics-digital-comics.png'
            //    },
            //    {
            //        text: 'Digital Comics',
            //        url: '#',
            //        image: '../assets/img/buy-comics-digital-comics.png'
            //    },
            //    {
            //        text: 'Digital Comics',
            //        url: '#',
            //        image: '../assets/img/buy-comics-digital-comics.png'
            //    },
            //    {
            //        text: 'Digital Comics',
            //        url: '#',
            //        image: '../assets/img/buy-comics-digital-comics.png'
            //    },
            //    {
            //        text: 'Digital Comics',
            //        url: '#',
            //        image: '../assets/img/buy-comics-digital-comics.png'
            //    }
            //]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";

#main-bottom{
    background-color: $secondaryColor;
    //height: 10vh;
    width: 100%;

    .container{
        @include container;

        ul{
            @include d-flex;
            justify-content: space-evenly;
            align-items: center;

            li a{
                @include d-flex;
                align-items: center;
                color: white;

                img{
                    width: 20%;
                    margin-right: 1rem;
                }

                p{
                    text-transform: uppercase;
                }
            }
        }
    }
}
</style>