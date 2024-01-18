<script>
    export default {
        data() {
            return { 
                 navigation: [
                    {
                        name: 'characters',
                        link: '#nogo',
                    },
                    {
                        name: 'comix',
                        link: '#nogo',
                    },
                    {
                        name: 'movies',
                        link: '#nogo',
                    },
                    {
                        name: 'tv',
                        link: '#nogo',
                    },
                    {
                        name: 'games',
                        link: '#nogo',
                    },
                    {
                        name: 'collectibles',
                        link: '#nogo',
                    },
                    {
                        name: 'videos',
                        link: '#nogo',
                    },
                    {
                        name: 'fans',
                        link: '#nogo',
                    },
                    {
                        name: 'news',
                        link: '#nogo',
                    },
                    {
                        name: 'shop',
                        link: '#nogo',
                    },
                 ],
            }
        },
    }
</script>

<template>
    <header class="">
        <div class="container">
            <div>
                <img src="../../public/img/dc-logo.png" alt="logo-dc-comics">
            </div>

            <nav>
                <ul>
                    <li class="nav-section" v-for="elem in navigation">
                        <a :href="elem.link">{{ elem.name }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
    @use "../assets/scss/header.scss" as *;
</style>
