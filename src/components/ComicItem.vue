<template>
    <div class="single-comic">
        <img class="comic-img" :src="ComicItemProps.thumb" :alt="ComicItemProps.series + ' image'">
        <h3 class="comic-title">{{ ComicItemProps.series }}</h3>
    </div>
</template>

<script>
export default {
    name: 'ComicItem',
    props: ['ComicItemProps']
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
    .single-comic{
        display: flex;
        flex-flow: column nowrap;
        justify-content: center;
        align-items: flex-start;

        width: calc( (100% / 6) - 10px );
        margin: 5px;
        .comic-img{
            width: 100%;
        }
        .comic-title{
            text-align: start;
            font-size: 16px;
            font-weight: 100;
            text-transform: uppercase;

            margin-top: 15px;
        }
    }
</style>