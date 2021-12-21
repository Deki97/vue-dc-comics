<template>
    <section>
        <div class="banner"></div>
    </section>
</template>


<script>
export default {
    name: 'Banner'
}
</script>


<style lang="scss" scoped>
section {
    .banner {
        width: 100%;
        background-image: url('../assets/img/jumbotron.jpg');
        height: 320px;
        background-position: top center;
        background-repeat: no-repeat;
        background-size: cover;
    }
}
</style>