<template>
    <div id="footer-bottom">
        <div class="container">
            <div class="sing-up">
                <a href="#">
                    Sign-up Now!
                </a>
            </div>
            <div class="social-icons">
                <h4>Follow us</h4>
                <a href="#" v-for="(element, index) in iconLinks" :key="index">
                    <img :src="require('../assets/img/' + element.image)" alt="Facebook Logo">
                </a>
            </div>
        </div>
        
    </div>
</template>

<script>
export default {
    name: 'FooterBottom',
    data: function(){
        return {
            iconLinks: [
                {
                    image: 'footer-facebook.png',
                    url: '#'
                },
                {
                    image: 'footer-twitter.png',
                    url: '#'
                },
                {
                    image: 'footer-youtube.png',
                    url: '#'
                },
                {
                    image: 'footer-pinterest.png',
                    url: '#'
                },
                {
                    image: 'footer-periscope.png',
                    url: '#'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";


#footer-bottom{
    height: calc(100% - 80%);
    background-color: #303030;
    padding: 1rem 0;

    div.container{
        @include container;
        @include d-flex;
        justify-content: space-between;
        align-items: center;
        height: 100%;

        .sing-up{
            
            a{
                display: inline-block;
                color: white;
                border: 2px solid $secondaryColor;
                padding: .7rem;
                text-transform: uppercase;
                font-weight: bold;
            }
        }

        .social-icons{
            @include d-flex;
            align-items: center;

            h4{
                text-transform: uppercase;
                color: $secondaryColor;
                font-weight: bold;
            }

            a {
                margin-left: 1rem;
            }

        }

    }
    
}

</style>