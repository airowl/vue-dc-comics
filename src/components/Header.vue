<template>
    <div id="header">
        <div class="main-logo">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
        </div>
        <nav class="header-nav">
            <ul>
                <li v-for="(link, index) in headerLinks" :key="index" :class="{ active: link.current}">
                    <a :href="link.url">{{link.text}}</a>
                </li>
                
            </ul>
        </nav>
    </div>
</template>

<script>
export default {
    name: 'mainHeader',
    data: function(){
        return {
            headerLinks: [
                {
                    text: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    text: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Tv',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Videos',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    text: 'News',
                    url: '#',
                    current: false,
                },
                {
                    text: 'Shop',
                    url: '#',
                    current: false,
                }
            ]
        }
    }
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

    nav.header-nav{
        
        height: 100%;

        ul{
            height: 100%;
            @include d-flex;
            justify-content: center;

            li{
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
                    color: $fontColor;
                    text-transform: uppercase;
                    font-size: .8rem;
                }
            }
        }
    }

}

</style>
