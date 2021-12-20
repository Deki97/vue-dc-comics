<template>
    <footer>
        Ciao sono il prefooter
    </footer>
</template>


<script>
export default {
    name: "PreFooter",
    data: function() {
        return {
            links: [
                {
                    imgUrl: '../assets/img/buy-comics-digital-comics.png',
                    text: 'DIGITAL COMICS',
                    url: '#'
                },
                {
                    imgUrl: '../assets/img/buy-comics-merchandise.png',
                    text: 'DC MERCHANDISE',
                    url: '#'
                },
                {
                    imgUrl: '../assets/img/buy-comics-subscriptions.png',
                    text: 'SUBSCRIPTION',
                    url: '#'
                },
                {
                    imgUrl: '../assets/img/buy-comics-shop-locator.png',
                    text: 'COMIC SHOP LOCATOR',
                    url: '#'
                },
                {
                    imgUrl: '../assets/img/buy-dc-power-visa.svg',
                    text: 'DC POWER VISA',
                    url: '#'
                }
            ]
        }
    }
}
</script>


<style lang="scss" scoped>

</style>