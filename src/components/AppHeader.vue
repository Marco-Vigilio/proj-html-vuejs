<template>
    <header>
        <div class="contain">
            <NavHeader />
            <JumbotronHeader />
        </div>
        <img class="face" src="../assets/img/home-movation-shape-face.png" alt="image of face draw">
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
@use '../style/partilas/variables' as*;

header {
    position: relative;
    background-image: url("../assets/img/background-pattern-wavify.png");
    background-color: $backGroundWaves;
    overflow: hidden;

    div.contain {
        max-width: 1170px;
        margin: 0 auto;
    }

    .face {
        position: absolute;
        margin-right: 1rem;
        width: 40%;
        top: 18rem;
        right: 0;
    }


}
</style>