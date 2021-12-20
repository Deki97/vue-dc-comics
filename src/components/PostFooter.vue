<template>
    <footer>
        Ciao sono il postfooter
    </footer>
</template>


<script>
export default {
    name: "PostFooter",
    data: function() {
        return {
            socials: [
                {
                    imgSrc: '../assets/img/footer-facebook.png',
                    url: '#'
                },
                {
                    imgSrc: '../assets/img/footer-twitter.png',
                    url: '#'
                },
                {
                    imgSrc: '../assets/img/footer-youtube.png',
                    url: '#'
                },
                {
                    imgSrc: '../assets/img/footer-pinterest.png',
                    url: '#'
                },
                {
                    imgSrc: '../assets/img/footer-periscope.png',
                    url: '#'
                }
            ]
        }
    }
}
</script>


<style lang="scss" scoped>

</style>