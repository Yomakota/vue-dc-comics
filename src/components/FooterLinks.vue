<template>
    <div class="container">
        <div class="col-left">
            
            <ul>
                <li v-for="element, index in dc_comics_list_links " :key="index">
                    <a href="">
                        {{ element.text }}
                    </a>
                </li>
            </ul>
            <ul>
                <li v-for="element, index in shop_list_links" :key="index">
                    <a href="">
                        {{ element.text }}
                    </a>
                </li>
            </ul>
            <ul>
                <li v-for="element, index in dc_list_links" :key="index">
                    <a href="">
                        {{ element.text }}
                    </a>
                </li>
            </ul>
            <ul>
                <li v-for="element, index in sites_list_links" :key="index">
                    <a href="">
                        {{ element.text }}
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name: 'FooterLinks',
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
    .container{
        background-image: url('../assets/img/footer-bg.jpg');
        display: flex;

        .col-left {
            display: flex;
        }

        li {
            display: flex;

            a{
                text-decoration: none;
                color: white;
            }
        }

    }
</style>