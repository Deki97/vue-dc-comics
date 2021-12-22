<template>
    <div class="comic">
        <div class="comic-image">
            <img :src="comicObject.thumb" :alt="comicObject.series">
        </div>

        <div class="comic-title">
            {{ comicObject.series }}
        </div>
    </div>
</template>


<script>
export default {
    name: 'SingleComic',
    props: ['comicObject']
}
</script>


<style lang="scss" scoped>
.comic {
    width: calc((100% / 6) - 20px);
    margin: 20px 10px;
    cursor: pointer;

    .comic-title {
        text-transform: uppercase;
        font-size: 12px;
        margin-top: 10px;
        text-align: left;
    }
}
</style>