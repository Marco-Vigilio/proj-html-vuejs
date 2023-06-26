<template>
    <div class="jumbotron">
        <div class="spot">
            qualcosa
        </div>
        <div class="my_image">
            immagine
        </div>
    </div>
</template>
<script>
export default {
    name: "Jumbotron Header",
}
</script>
<style lang="scss" scoped>
.jumbotron {
    display: flex;

    div.my_image,
    div.spot {
        width: calc(100% / 2);
        height: 300px;
    }

    .spot {
        background-color: red;
        border: 2px solid black;
    }

    .my_image {
        background-color: green;
        border: 2px solid black;
    }

}
</style>