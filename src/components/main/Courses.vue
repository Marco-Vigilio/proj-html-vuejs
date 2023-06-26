<template>
    <section>
        <div class="title">Titolo</div>
        <div class="cards">
            <Card />
        </div>
        <div class="button">
            <button class="button">Vedi tutti i corsi</button>
        </div>
    </section>
</template>
<script>
import Card from './Card.vue';
export default {
    name: "Courses",
    components: {
        Card,
    }
}
</script>
<style lang="scss" scoped>
div.title {
    text-align: center;
}

.cards {
    display: flex;
}

.button {
    display: flex;
    justify-content: center;
}
</style>