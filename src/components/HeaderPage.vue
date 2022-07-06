<template>
    <header>
        <div class="container">
            <img src="../assets/img/dc-logo.png" alt="">
            <ul>
                <li v-for="link, index in links" :key="index">
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
            links: [
                {
                    name: 'Characters',
                    url: '#',
                },
                {
                    name: 'Comics',
                    url: '#',
                },
                {
                    name: 'Movies',
                    url: '#',
                },
                {
                    name: 'TV',               url: '#',
                },
                {
                    name: 'Game',
                    url: '#',
                },
                {
                    name: 'Collectibles',
                    url: '#',
                },
                {
                    name: 'Videos',
                    url: '#',
                },
                {
                    name: 'Fans',
                    url: '#',
                },
                {
                    name: 'News',
                    url: '#',
                },
                {
                    name: 'Shop',
                    url: '#',
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
header {
    width: 100%;
    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;

        img {
            width: 100px;
        }

        ul {
            display: flex;

            li {
                display: flex;
                text-transform: uppercase;
                margin: 0 1em;

                a {
                    text-decoration: none;
                    color: black;
                }
            }
        }
    }
}
</style>