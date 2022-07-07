<template>
    <section class="footer-bottom">
        <div class="container">
            <div class="col-left">
                <button>
                    <a href="">
                        sign up now!
                    </a>
                </button>
            </div>
            <div class="col-right">
                <h3>
                    Follow Us
                </h3>
                <ul>
                    <li v-for="social, index in socials" :key="index">
                        <a :href="social.url">
                            <img :src="social.icon" :alt="social.name">
                        </a>
                    </li>
                </ul>
                <!-- <ul>
                    <li>
                        <img src="../assets/img/footer-facebook.png" alt="">
                    </li>
                    <li>
                        <img src="../assets/img/footer-twitter.png" alt="">
                    </li>
                    <li>
                        <img src="../assets/img/footer-youtube.png" alt="">
                    </li>
                    <li>
                        <img src="../assets/img/footer-pinterest.png" alt="">
                    </li>
                    <li>
                        <img src="../assets/img/footer-periscope.png" alt="">
                    </li>
                 </ul> -->
            </div>
        </div>
   </section>
</template>

<script>
export default {
    name: 'FooterBottom',
    data() {
        return {
            socials: [
                {   
                    name:'facebook',
                    icon: require('../assets/img/footer-facebook.png'),
                    url:'#',
                },
                {
                    name: 'twitter',
                    icon: require('../assets/img/footer-twitter.png'),
                    url: '#',
                },
                {   name:'youtube',
                    icon: require('../assets/img/footer-youtube.png'),
                    url: '#',
                },
                {   
                    name:'pintarest',
                    icon: require('../assets/img/footer-pinterest.png'),
                    url: '#',
                },
                {
                    name:'periscope',
                    icon: require('../assets/img/footer-periscope.png'),
                    url: '#',
                }
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";

.footer-bottom{
    background-color: $footerBottom;
    .container {
        display: flex;
        justify-content: space-around;
        align-items: center;
        text-transform: uppercase;
        .col-left {
            button {
                border: 1px solid blue;
                padding: 10px;
                background-color: transparent;
                text-transform: uppercase;
                a{
                    color: white;
                }
            }
        }
        .col-right{
            display: flex;
            justify-content: space-around;
            align-items: center;
            h3{
                color: $bottomLink;
            }
            ul{
                display: flex;
                li{
                    display: flex;
                    padding: 10px;
                }
            }
        }
    }
}
</style>