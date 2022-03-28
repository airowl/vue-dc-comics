<template>
    <div id="footer">
        <div id="footer-top">

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

    #footer-top{
        height: 80%;
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
}

</style>