<template>
    <section class="postfooter">
        <div class="container">
            <div class="signup-col">
                <div class="btn-signup">
                    <a href="#">SIGN-UP NOW!</a>
                </div>
            </div>

            <div class="socials-col">
                <div class="follow-us">
                    FOLLOW US
                </div>

                <div class="social-icons">
                    <ul>
                        <li v-for="(icon, index) in socials" :key="index">
                            <a :href="icon.url">
                                <img :src="icon.imgSrc" :alt="icon.name">
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>


<script>
export default {
    name: "PostFooter",
    data: function() {
        return {
            socials: [
                {
                    imgSrc: require('../assets/img/footer-facebook.png'),
                    url: '#',
                    name: 'Facebook'
                },
                {
                    imgSrc: require('../assets/img/footer-twitter.png'),
                    url: '#',
                    name: 'Twitter'
                },
                {
                    imgSrc: require('../assets/img/footer-youtube.png'),
                    url: '#',
                    name: 'Youtube'
                },
                {
                    imgSrc: require('../assets/img/footer-pinterest.png'),
                    url: '#',
                    name: 'Pinterest'
                },
                {
                    imgSrc: require('../assets/img/footer-periscope.png'),
                    url: '#',
                    name: 'Periscope'
                }
            ]
        }
    }
}
</script>


<style lang="scss" scoped>
.postfooter {
    background-color: #303030;
    padding: 30px 0;
}

.container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    .btn-signup {
        font-size: 15px;
        border: 3px solid #0282f9;
        display: inline-block;
        padding: 8px;
        color: white;
    }

    .socials-col {
        display: flex;
        align-items: center;

        .follow-us {
            font-weight: 700;
            color: #0282f9;
            padding-right: 20px;
        }

        .social-icons ul li {
            display: inline-block;
            padding: 0 10px;

            img {
                width: 30px;
            }
        }
    }
}
</style>