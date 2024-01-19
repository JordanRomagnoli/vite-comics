<script>

    export default {
        data() {
            return { 

            }
        },
        props: {
            product: Object,
            image: String,
            prizing: String,
            serial: String,
            typo: String,
        },
    }
    </script>

<template>
    <div class="comix-frame">
        <div>
            <img :src="image" :alt="serial">
        </div>
        <span>{{ serial }}</span>
    </div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables" as *;
@use "../assets/scss/partials/mixins" as *;

.comix-frame{
    @include nav-text;
    width: calc(100% / 6);
    margin-bottom: 50px;
    text-align: center;

    > div{
        width: 180px;
        height: 220px;
        border-radius: 10px;
        border: 1px solid white;
        overflow: hidden;
        margin: 0 auto;
        margin-bottom: 10px;
        cursor: pointer;

        > img{
            width: 100%;
        }
    }
}
    
</style>
