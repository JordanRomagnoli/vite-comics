<script>

/*
    Importazione componente
*/
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
    data() {
        return { 
             
        }
    },
    /*
        Dichiarazione dei componenti all'interno dell'oggetto
    */
    components: {

        AppHeader,
        AppMain,
        AppFooter
    },
}
</script>

<template>
    
    <!--
        Utilizzo del componente
    -->
    <AppHeader/>
    <AppMain/>
    <AppFooter/>
        
    
</template>

<style lang="scss" scoped>
</style>
