<template >
    <div class="jumbotron">
        <section>
            <span>REAL STORIES</span>
            Storie
        </section>
        <section>
            immagine
        </section>
    </div>
</template>
<script>
export default {
    name: "Jumbotron",
}
</script>
<style lang="scss" scoped>
div.jumbotron {
    background-color: gold;
    display: flex;

    section {
        display: flex;
        justify-content: center;
        width: calc(100% / 2);
    }
}
</style>