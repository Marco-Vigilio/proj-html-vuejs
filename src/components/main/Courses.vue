<template>
    <section>
        <div class="title">
            <span>BEGIN YOUR JOURNEY AT MAXCOACH</span>
            <h2>Latest Online Courses</h2>
        </div>
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
    padding-bottom: 2rem;

    h2 {
        font-size: 2.5rem;
    }
}

.cards {
    display: flex;
}

.button {
    display: flex;
    justify-content: center;
    border: none;
    padding: 1rem 4rem;
    border-radius: .3rem;
}
</style>