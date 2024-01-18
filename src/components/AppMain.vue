<script>
    export default {
        data() {
            return { 

                sectionLink: [
                    {
                        img: '../../public/img/buy-comics-digital-comics.png',
                        name: 'digital comics',
                        link: '#nogo',
                    },
                    {
                        img: '../../public/img/buy-comics-merchandise.png',
                        name: 'dc merchandise',
                        link: '#nogo',
                    },
                    {
                        img: '../../public/img/buy-comics-subscriptions.png',
                        name: 'subscription',
                        link: '#nogo',
                    },
                    {
                        img: '../../public/img/buy-comics-shop-locator.png',
                        name: 'comic shop locator',
                        link: '#nogo',
                    },
                    {
                        img: '../../public/img/buy-dc-power-visa.svg',
                        name: 'dc power visa',
                        link: '#nogo',
                    },
                ],
            }
        },
    }
    </script>

<template>
    <div class="main-top">
        <div class="container">
            <div>
                <h2>
                    Content goes here
                </h2>
            </div>
        </div>
    </div>

    <div class="main-bottom">
        <div class="container">
            <ul>
                <li v-for="elem in sectionLink">
                    <a :href="elem.link">
                        <div class="img-frame">
                        <img :src="elem.img" :alt="elem.name">
                        </div>

                        <span>
                            {{ elem.name }}
                        </span>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    @use "../assets/scss/main.scss" as *;
</style>
