<template>
    <main>
        <div class="container">
            <ul>
                <li v-for="link, index in links" :key="index">
                    <a :href="link.url">
                        <div class="image-link">
                            <img :src="link.image" :alt="link.text">
                        </div>
                        <div class="text-link">
                            {{link.text}}
                        </div>
                    </a>
                </li>
            </ul>
            <!-- <ul>
                <li>
                    <a href="">
                        <div>
                            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        </div>
                        <div class="text-link">
                            digital comics
                        </div>
                    </a>
                </li>
                <li>
                    <a href="">
                        <div>
                            <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        </div>
                        <div class="text-link">
                            dc merchandise
                        </div>
                    </a>
                </li>
                <li>
                    <a href="">
                        <div>
                            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        </div>
                        <div class="text-link">
                            subscriction
                        </div>
                    </a>
                </li>
                <li>
                    <a href="">
                        <div>
                            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                        </div>
                        <div class="text-link">
                            comic shop locator
                        </div>
                    </a>
                </li>
                <li>
                    <a href="">
                        <div class="image-link">
                            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                        </div>
                        <div class="text-link">
                            dc power visa
                        </div>
                    </a>
                </li>
            </ul> -->
        </div>
    </main>
</template>

<script>
export default {
    name: 'MainMenu',
    data() {
        return {
            links: [
                {
                    text: 'digital comics',
                    image: require('../assets/img/buy-comics-digital-comics.png'),
                    url: '#',
                },
                {
                    text: 'dc merchandise',
                    image: require('../assets/img/buy-comics-merchandise.png'),
                    url: '#',
                },
                {
                    text: 'subscription',
                    image: require('../assets/img/buy-comics-subscriptions.png'),
                    url: '#',
                },
                {
                    text: 'comic shop locator',
                    image: require('../assets/img/buy-comics-shop-locator.png'),
                    url: '#',
                },
                {
                    text: 'dc power visa',
                    image: require('../assets/img/buy-dc-power-visa.svg'),
                    url: '#',
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";

main {
    background-color: $mainMenu;
    .container {
        padding: 2em;

        ul {
            display: flex;
            justify-content: space-between;

            a {
                display: flex;
                align-items: center;
                color: white;
                text-transform: uppercase;
                text-decoration: none;

                img {
                    height: 50px;
                }

                .text-link {
                    padding: .5em;
                    font-size: .5em;
                }
                .image-link {
                    width: 40px;
                }
            }
        }
    }
}
</style>