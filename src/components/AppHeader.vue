<script>
    export default {
        data() {
            return { 
                 navigation: [
                    {
                        name: 'characters',
                        link: '#nogo',
                        active: false,
                    },
                    {
                        name: 'comix',
                        link: '#nogo',
                        active: false ,
                    },
                    {
                        name: 'movies',
                        link: '#nogo',
                        active: false ,
                    },
                    {
                        name: 'tv',
                        link: '#nogo',
                        active: false ,
                    },
                    {
                        name: 'games',
                        link: '#nogo',
                        active: false ,
                    },
                    {
                        name: 'collectibles',
                        link: '#nogo',
                        active: false ,
                    },
                    {
                        name: 'videos',
                        link: '#nogo',
                        active: false ,
                    },
                    {
                        name: 'fans',
                        link: '#nogo',
                        active: false ,
                    },
                    {
                        name: 'news',
                        link: '#nogo',
                        active: false ,
                    },
                    {
                        name: 'shop',
                        link: '#nogo',
                        active: false ,
                    },
                 ],
            }
        },
        methods:{
            activeMenu(element){
                for(let i = 0; i < this.navigation.length; i++){
                    this.navigation[i].active = false;
                }

                element.active = !element.active
            },
        },
    }
</script>

<template>
    <header>
        <div class="container">
            <div>
                <img src="../../public/img/dc-logo.png" alt="logo-dc-comics">
            </div>

            <nav>
                <ul>
                    <li class="nav-section" v-for="(elem, index) in navigation" :key="elem">
                        <a :href="elem.link" 
                        :class="{
                            'active': elem.active
                        }"
                        @click="activeMenu(elem)">{{ elem.name }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
    @use "../assets/scss/header.scss" as *;
</style>
