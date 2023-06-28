<template>
    <header>
        <div class="view">
            <div class="contain">
                <NavHeader />
            </div>
        </div>

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
    },
    data() {
        return {
        }
    },
}
</script>
<style lang="scss" scoped>
@use '../style/partilas/variables' as*;

header {
    position: relative;
    background-image: url("../assets/img/background-pattern-wavify.png");
    background-color: $backGroundWaves;
    overflow: hidden;

    div.view {
        background-color: white;
        width: 100%;
        position: fixed;
        z-index: 2;
        box-shadow: 0 0 25px rgba(0, 0, 0, 0.2);
        display: none;
    }

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