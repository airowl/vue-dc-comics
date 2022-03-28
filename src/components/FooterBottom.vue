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
                <a href="#">
                    <img src="../assets/img/footer-facebook.png" alt="Facebook Logo">
                </a>
                <a href="#">
                    <img src="../assets/img/footer-twitter.png" alt="Twitter Logo">
                </a>
                <a href="#">
                    <img src="../assets/img/footer-youtube.png" alt="Youtube Logo">
                </a>
                <a href="#">
                    <img src="../assets/img/footer-pinterest.png" alt="Pinterest Logo">
                </a>
                <a href="#">
                    <img src="../assets/img/footer-periscope.png" alt="Periscope Logo">
                </a>
            </div>
        </div>
        
    </div>
</template>

<script>
export default {
    name: 'FooterBottom'
}
</script>

<style lang="scss" scoped>
@import "../assets/scss/style.scss";


#footer-bottom{
    height: calc(100% - 80%);
    background-color: #303030;

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

            a {
                margin-left: 1rem;
            }

        }

    }
    
}

</style>