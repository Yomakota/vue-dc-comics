<template>
    <section class="footer-top">
        <div class="container">
            <div class="col-left">
                <div class="col-1">
                    <ul>
                        <h3>Dc comics</h3>
                        <li v-for="element, index in dc_comics_list_links " :key="index">
                            <a href="">
                                {{ element.text }}
                            </a>
                        </li>
                    </ul>
                    <ul>
                        <h3>Shop</h3>
                        <li v-for="element, index in shop_list_links" :key="index">
                            <a href="">
                                {{ element.text }}
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="col-2">
                    <ul>
                        <h3>DC</h3>
                        <li v-for="element, index in dc_list_links" :key="index">
                            <a href="">
                                {{ element.text }}
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="col-3">
                    <ul>
                        <h3>Sites</h3>
                        <li v-for="element, index in sites_list_links" :key="index">
                            <a href="">
                                {{ element.text }}
                            </a>
                        </li>
                    </ul>
                </div>
            </div>
            <div class="col-right">
               
            </div>
        </div>

    </section>
</template>

<script>
export default {
    name: 'FooterTop',
    data() {
        return {
            dc_comics_list_links: [
                {
                    text: 'Characters',
                    url: '#',
                },
                {
                    text: 'Comics',
                    url: '#',
                },
                {
                    text: 'Movies',
                    url: '#',
                },
                {
                    text: 'TV',
                    url: '#',
                },
                {
                    text: 'Games',
                    url: '#',
                },
                {
                    text: 'Videos',
                    url: '#',
                }, {
                    text: 'News',
                    url: '#',
                },
            ],
            shop_list_links: [
                {
                    text: 'Shop DC',
                    url: '#',
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#',
                },
            ],
            dc_list_links: [
                {
                    text: 'Terms Of Use',
                    url: '#',
                },
                {
                    text: 'Privacy policy(News)',
                    url: '#',
                },
                {
                    text: 'Ad Choices',
                    url: '#',
                },
                {
                    text: 'Advertising',
                    url: '#',
                },
                {
                    text: 'Jobs',
                    url: '#',
                },
                {
                    text: 'Subscriptions',
                    url: '#',
                }, {
                    text: 'Talent Workshops',
                    url: '#',
                },
                {
                    text: 'CPSC Certificates',
                    url: '#',
                },
                {
                    text: 'Ratings',
                    url: '#',
                },
                {
                    text: 'Shop Help',
                    url: '#',
                }, {
                    text: 'Contact Us',
                    url: '#',
                },
            ],
            sites_list_links: [
                {
                    text: 'DC',
                    url: '#',
                },
                {
                    text: 'MAD Magazine',
                    url: '#',
                },
                {
                    text: 'DC Kids',
                    url: '#',
                },
                {
                    text: 'DC Universe',
                    url: '#',
                },
                {
                    text: 'DC Power Visa',
                    url: '#',
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
.footer-top {
    display: flex;
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    font-size: 10px;

    .container {
        display: flex;
        justify-content: space-between;
        .col-left {
            display: flex;

            ul {
                display: flex;
                flex-direction: column;
                padding: 2em;
                h3{
                    color: white;
                    font-weight: 700;
                    font-size: 15px;
                    text-transform: uppercase;
                    padding-bottom: 10px;
                }
                li {
                    display: flex;
                    padding-bottom: 5px;
                    a {
                        text-decoration: none;
                        color: $footerLink;
                    }
                }
            }
        }
        .col-right {
            background-image: url(../assets/img/dc-logo-bg.png);
            background-size: cover;
            background-position: center;
            width: 40%;
        }   
    }
}
</style>