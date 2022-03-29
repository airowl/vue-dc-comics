<template>
    <div id="main-bottom">
        <div class="container">
            <ul>
                <li v-for="(element, index) in mainBottomLinks" :key="index">
                    <a :href="element.url">
                        <img :src="require('../assets/img/' + element.image)" alt="">
                        <p>{{element.text}}</p>
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
            mainBottomLinks: [
                {
                    text: 'Digital Comics',
                    url: '#',
                    image: 'buy-comics-digital-comics.png'
                },
                {
                    text: 'Merchandise',
                    url: '#',
                    image: 'buy-comics-merchandise.png'
                },
                {
                    text: 'Shop Locator',
                    url: '#',
                    image: 'buy-comics-shop-locator.png'
                },
                {
                    text: 'Subscriptions',
                    url: '#',
                    image: 'buy-comics-subscriptions.png'
                },
                {
                    text: 'Power Visa',
                    url: '#',
                    image: 'buy-dc-power-visa.svg'
                }
            ]
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
            padding: 2rem 0;

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