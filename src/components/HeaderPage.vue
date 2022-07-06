<template>
    <header>
        <div class="container">
            <img src="../assets/img/dc-logo.png" alt="">
            <ul>
                <li v-for="link, index in links" 
                    :key="index" 
                    :class="{'active': link.active}"
                >
                    <a :href="link.url">
                        {{ link.name }}
                    </a>
                </li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
    name: 'HeaderPage',
    data() {
        return {
            activeElement: null,
            links: [
                {
                    name: 'Characters',
                    url: '#',
                    active:false,
                },
                {
                    name: 'Comics',
                    url: '#',
                    active: true,
                },
                {
                    name: 'Movies',
                    url: '#',
                    active: false,
                },
                {
                    name: 'TV', 
                    url: '#',
                    active: false,
                },
                {
                    name: 'Game',
                    url: '#',
                    active: false,
                },
                {
                    name: 'Collectibles',
                    url: '#',
                    active: false,
                },
                {
                    name: 'Videos',
                    url: '#',
                    active: false,
                },
                {
                    name: 'Fans',
                    url: '#',
                    active: false,
                },
                {
                    name: 'News',
                    url: '#',
                    active: false,
                },
                {
                    name: 'Shop',
                    url: '#',
                    active: false,
                },
            ],
        }
    },
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";
header {
    background-color: white;
    width: 100%;
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;

        img {
            width: 100px;
            padding: .5em;
        }

        ul {
            display: flex;

            li {
                display: flex;
                text-transform: uppercase;
                font-size: .7em;
                margin: 0 1em;
                height: 100%;
                line-height: 94px;

                // &:hover,
                &.active{
                        color: $activeMenu;
                        border-bottom: 1px solid $activeMenu;
                        border-bottom-width: 10px;
                    }

                a {
                    text-decoration: none;
                    color: black;
                }
            }
        }
    }
}
</style>