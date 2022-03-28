<template>
    <div id="header">
        <div class="main-logo">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
        </div>
        <nav class="header-nav">
            <ul>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Characters</a></li>
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
    border: 1px solid red;

    nav.header-nav{
        
        ul{
            @include d-flex;

            li{
                list-style-type: none;

                a{
                    text-decoration: none;
                    color: $fontColor;
                }
            }
        }
    }

}

</style>
