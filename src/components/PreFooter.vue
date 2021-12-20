<template>
    <section class="prefooter">
        <div class="container">
            <div class="single-link" v-for="(link, index) in links" :key="index">
                <div class="link-image">
                    <img :src="link.imgUrl" :alt="link.text">
                </div>
                <div class="link-text">
                    <a :href="link.url">
                        {{ link.text }}
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    name: "PreFooter",
    data: function() {
        return {
            links: [
                {
                    imgUrl: require('../assets/img/buy-comics-digital-comics.png'),
                    text: 'DIGITAL COMICS',
                    url: '#'
                },
                {
                    imgUrl: require('../assets/img/buy-comics-merchandise.png'),
                    text: 'DC MERCHANDISE',
                    url: '#'
                },
                {
                    imgUrl: require('../assets/img/buy-comics-subscriptions.png'),
                    text: 'SUBSCRIPTION',
                    url: '#'
                },
                {
                    imgUrl: require('../assets/img/buy-comics-shop-locator.png'),
                    text: 'COMIC SHOP LOCATOR',
                    url: '#'
                },
                {
                    imgUrl: require('../assets/img/buy-dc-power-visa.svg'),
                    text: 'DC POWER VISA',
                    url: '#'
                }
            ]
        }
    }
}
</script>


<style lang="scss" scoped>
.prefooter {
    background-color: #0282f9;
    color: white;

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 30px 0;

        .single-link {
            display: flex;
            align-items: center;

            .link-image {
                width: 40px;
            }

            .link-text {
                font-size: 12px;
                margin-left: 10px;
            }
        }
    }
}
</style>