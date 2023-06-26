<script >
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import AppMain from './components/AppMain.vue';
export default {
    components: {
        AppHeader,
        AppMain,
        AppFooter,
    },
}

</script>

<template>
    <AppHeader />
    <AppMain />
    <AppFooter />
</template>

<style lang="scss">
@import './style/generals.scss';

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

ul {
    list-style: none;
}
</style>
