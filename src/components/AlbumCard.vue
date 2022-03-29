<template>
    <div class="album-card">
        <div class="album-image">
            <img :src="singleCard.thumb" :alt="singleCard.series">
        </div>
        <h4>{{singleCard.series}}</h4>
    </div>
</template>

<script>
export default {
    name: 'albumCard',
    props: {
        singleCard: Object
    }
}
</script>

<style lang="scss" scoped>
    div.album-card{
            width: calc((100% / 6) - 1rem);
            text-align: start;
            
            h4{
                margin:  1rem 0;
                text-transform: uppercase;
            }

            div.album-image{
                width: 100%;
                height: 12rem;
                overflow: hidden;

                img{
                    width: 100%;
                }
            }
        }
</style>