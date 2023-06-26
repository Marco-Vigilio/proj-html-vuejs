<template>
    <div class="card">
        <div class="header">
            <img :src="image" alt="image of couse">
        </div>
        <div class="main">
            <span>&dollar;{{ priceNumber }}</span>
            <span>.{{ priceNumberDecimal }}</span>
            <p>{{ name }}</p>
        </div>
        <div class="footer">
            <span v-if="numLesson === '1'">
                <i class="fa-regular fa-file-lines"></i>
                {{ numLesson }} Lesson
            </span>
            <span v-else>
                <i class="fa-regular fa-file-lines"></i>
                {{ numLesson }} Lessons
            </span>

            <span>
                <i class="fa-regular fa-user"></i>
                {{ numStudents }} Students
            </span>
        </div>
    </div>
</template>
<script>
export default {
    name: "Card",
    props: {
        name: String,
        priceNumber: String,
        priceNumberDecimal: String,
        image: String,
        numLesson: String,
        numStudents: String,
    },
    data() {
        return {

        }
    },
    methods: {
        price() {
            console.log(this.name);
        }
    },
    /*
    mounted() {
        this.price(price);
    },
    */
}
</script>
<style lang="scss" scoped>
.card {
    width: (calc(100% / 3)-2);
    border: 2px solid black;

    header {
        width: 100%;

        img {
            width: 100%;
        }
    }
}
</style>