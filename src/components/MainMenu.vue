<template>
    <div class="container">
        <ul>
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
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    </div>
                    <div class="text-link">
                        subscriction
                    </div>
                </a>
            </li>
            <li>
                <a href="">
                    <div>
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    </div>
                    <div class="text-link">
                        comic shop locator
                    </div>
                </a>
            </li>
            <li>
                <a href="">
                    <div>
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    </div>
                    <div class="text-link">
                        dc power visa
                    </div>
                </a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'MainMenu',
    data() {
        return {
            // links: [
            //     {
            //         image: '../assets/img/buy-comics-digital-comics.png',
            //         url: '#',
            //         text: 'testo link',
            //     },
            //     {
            //         image: '../assets/img/buy-comics-merchandise.png',
            //         url: '#',
            //     },
            //     {
            //         image: '../assets/img/buy-comics-shop-locator.png',
            //         url: '#',
            //     },
            //     {
            //         image: '../assets/img/buy-comics-subscriptions.png',
            //         url: '#',
            //     },
            //     {
            //         image: '../assets/img/buy-dc-power-visa.svg',
            //         url: '#',
            //     },
            // ],
        }
    }
}
</script>

<style lang="scss" scoped>
.container {
    background-color: lightblue;
    ul {
        display: flex;
        justify-content: space-around;
        padding: 2em;

        li {
            display: flex;

            a {
                display: flex;
                align-items: center;
                color: white;
                text-transform: uppercase;
                text-decoration: none;

                img {
                    height: 50px;
                    margin-right: 10px;
                }
            }
        }
    }
}
</style>