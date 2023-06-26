<template>
    <section>
        <div class="introduction">
            <article>About Me</article>
            <article>Articolo</article>
        </div>
        <div class="about">
            <article class="video">Video</article>
            <article>qualcosa</article>
        </div>
    </section>
</template>
<script>
export default {
    name: "About Me",
}
</script>
<style lang="scss" scoped>
section {
    .introduction {
        display: flex;

        article {
            border: 2px solid black;
            background-color: red;
            width: calc(100% / 2);
            display: flex;
            justify-content: center;
        }
    }

    .about {
        display: flex;

        article.video {
            background-color: violet;
            width: 60%;
        }

        //no margin, PADDING
    }
}
</style>