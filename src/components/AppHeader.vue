<template>
    <header>
        <div class="contain">
            <NavHeader />
            <JumbotronHeader />
        </div>
    </header>
</template>
<script>
import NavHeader from './header/NavHeader.vue';
import JumbotronHeader from './header/JumbotronHeader.vue';
export default {
    name: "Header",
    components: {
        NavHeader,
        JumbotronHeader,
    }
}
</script>
<style lang="scss" scoped>
header {
    background-image: url("../assets/img/background-pattern-wavify.png");
    background-color: gold;

    div.contain {
        max-width: 1170px;
        margin: 0 auto;
    }


}
</style>