<template>
    <footer>
        <div class="container">
            <div class="cols">
                <div class="col-comics-shop">
                    <div class="col-comics">
                        <div class="title">
                            <h3>DC COMICS</h3>
                        </div>

                        <div class="col-list">
                            <ul>
                                <li v-for="(link, index) in dc_comics" :key="index">
                                    <a :href="link.url">
                                        {{ link.text }}
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>

                    <div class="col-shop">
                        <div class="title">
                            <h3>SHOP</h3>
                        </div>

                        <div class="col-list">
                            <ul>
                                <li v-for="(link, index) in shop" :key="index">
                                    <a :href="link.url">
                                        {{ link.text }}
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>

                <div class="col-dc">
                    <div class="title">
                        <h3>DC</h3>
                    </div>

                    <div class="col-list">
                        <ul>
                            <li v-for="(link, index) in dc" :key="index">
                                <a :href="link.url">
                                    {{ link.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>

                <div class="col-sites">
                    <div class="title">
                        <h3>SITES</h3>
                    </div>

                    <div class="col-list">
                        <ul>
                            <li v-for="(link, index) in sites" :key="index">
                                <a :href="link.url">
                                    {{ link.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>

            <div class="footer-logo">
                <img src="../assets/img/dc-logo-bg.png" alt="DC Logo">
            </div>
        </div>
    </footer>
</template>


<script>
export default {
    name: "Footer",
    data: function() {
        return {
            dc_comics: [
                {
                    text: 'Characters',
                    url: '#'
                },
                {
                    text: 'Comics',
                    url: '#'
                },
                {
                    text: 'Movies',
                    url: '#'
                },
                {
                    text: 'TV',
                    url: '#'
                },
                {
                    text: 'Games',
                    url: '#'
                },
                {
                    text: 'Videos',
                    url: '#'
                },
                {
                    text: 'News',
                    url: '#'
                }
            ],
            shop: [
                {
                    text: 'Shop DC',
                    url: '#'
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#'
                }
            ],
            dc: [
                {
                    text: 'Terms Of Use',
                    url: '#'
                },
                {
                    text: 'Privacy policy (New)',
                    url: '#'
                },
                {
                    text: 'Ad Choices',
                    url: '#'
                },
                {
                    text: 'Advertising',
                    url: '#'
                },
                {
                    text: 'Jobs',
                    url: '#'
                },
                {
                    text: 'Subscriptions',
                    url: '#'
                },
                {
                    text: 'Talent Workshops',
                    url: '#'
                },
                {
                    text: 'CPSC Certificates',
                    url: '#'
                },
                {
                    text: 'Ratings',
                    url: '#'
                },
                {
                    text: 'Shop Help',
                    url: '#'
                },
                {
                    text: 'Contact Us',
                    url: '#'
                }
            ],
            sites: [
                {
                    text: 'DC',
                    url: '#'
                },
                {
                    text: 'MAD Magazine',
                    url: '#'
                },
                {
                    text: 'DC Kids',
                    url: '#'
                },
                {
                    text: 'DC Universe',
                    url: '#'
                },
                {
                    text: 'DC Power Visa',
                    url: '#'
                }
            ]
        }
    }
}
</script>


<style lang="scss" scoped>
footer {
    background-image: url('../assets/img/footer-bg.jpg');
    padding: 15px 0 40px 0;
    background-repeat: no-repeat;
    background-size: cover;
    max-height: 320px;
}

.container {
    display: flex;
    justify-content: space-between;
    position: relative;

    .cols {
        display: flex;

        &>div {
            margin-right: 30px;
        }

        .title h3 {
            font-size: 16px;
            letter-spacing: -1px;
            margin-top: 20px;
            color: white;
        }

        .col-list ul {
            margin: 5px 0;
        }

        .col-list a {
            font-size: 12px;
            color: #898481;
        }
    }

    .footer-logo {
        width: 450px;
        position: absolute;
        top: -30%;
        right: 0;
    }
}

</style>