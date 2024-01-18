<script>
    export default {
        data() {
            return { 
                navigation1: [
                    {
                        name: 'Characters',
                    },
                    {
                        name: 'Comix',
                    },
                    {
                        name: 'Movies',
                    },
                    {
                        name: 'Tv',
                    },
                    {
                        name: 'Games',
                    },
                    {
                        name: 'Videos',
                    },
                    {
                        name: 'News',
                    }
                ],
                navigation2: [
                    {
                        name: 'Shop DC',
                    },
                    {
                        name: 'Shop DC Collectibles',
                    }
                ],
                navigation3: [
                    {
                        name: 'Terms Of Use',
                    },
                    {
                        name: 'Privacy Policy (News)',
                    },
                    {
                        name: 'Ad Choice',
                    },
                    {
                        name: 'Advertising',
                    },
                    {
                        name: 'Jobs',
                    },
                    {
                        name: 'Subscriptions',
                    },
                    {
                        name: 'Talent Workshops',
                    },
                    {
                        name: 'CPSC Certificates',
                    },
                    {
                        name: 'Ratings',
                    },
                    {
                        name: 'Shop Help',
                    },
                    {
                        name: 'Contact Us',
                    },
                ],
                navigation4: [
                    {
                        name: 'DC',
                    },
                    {
                        name: 'MAD Magazine',
                    },
                    {
                        name: 'DC Kids',
                    },
                    {
                        name: 'DC Universe',
                    },
                    {
                        name: 'DC Power Visa',
                    }
                ],
                socialList: [
                    {
                        img: '../../public/img/footer-facebook.png',
                    },
                    {
                        img: '../../public/img/footer-twitter.png',
                    },
                    {
                        img: '../../public/img/footer-youtube.png',
                    },
                    {
                        img: '../../public/img/footer-pinterest.png',
                    },
                    {
                        img: '../../public/img/footer-periscope.png',
                    },

                ],
            }
        },
    }
    </script>

<template>
    <section class="footer-top">
        <div class="container">
            <ul>
                <li>
                    <div>
                        <h3>dc comix</h3>
                        <ul>
                            <li v-for="elem in navigation1">
                                <a href="#nogo">{{ elem.name }}</a>
                            </li>
                        </ul>
                    </div>

                    <div>
                        <h3>shop</h3>
                        <ul>
                            <li v-for="elem in navigation2">
                                <a href="#nogo">{{ elem.name }}</a>
                            </li>
                        </ul>
                    </div>
                </li>
                
                <li>
                    <h3>dc</h3>
                    <ul>
                        <li v-for="elem in navigation3">
                            <a href="#nogo">{{ elem.name }}</a>
                        </li>
                    </ul>
                </li>

                <li>
                    <h3>sites</h3>
                    <ul>
                        <li v-for="elem in navigation4">
                            <a href="#nogo">{{ elem.name }}</a>
                        </li>
                    </ul>
                </li>
            </ul>

            <div class="lg-img-frame">
                
            </div>
        </div>
    </section>

    <section class="footer-bottom">
        <div class="container">
            <a href="#nogo">sign-up now!</a>

            <div class="social-container">
                <span>
                    follow us
                </span>
                <ul>
                    <li v-for="elem in socialList">
                        <a href="#nogo"><img :src="elem.img" alt=""></a>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    @use "../assets/scss/footer.scss" as *;
</style>
