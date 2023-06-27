<template>
    <div class="card">
        <div class="header">
            <img :src="image" alt="image of couse">
        </div>
        <div class="contain">
            <div class="main">
                <span class="green">&dollar;{{ priceNumber }}</span>
                <span class="green">.{{ priceNumberDecimal }}</span>
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
        numLesson: Number,
        numStudents: Number,
    },
    data() {
        return {
            numDecimal: "",
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
@use '../../style/partilas/variables' as*;

span.green {
    color: $green;
}

.card {
    width: (calc((100% - 4rem) / 3));
    border-radius: .4rem;
    overflow: hidden;

    .contain {
        padding: 1rem 2rem;

        .header {
            width: 100%;

            img {
                width: 100%;
                display: block;
            }
        }

        .main {
            span:first-child {
                font-size: 1.5rem;
            }

            p {
                font-size: 1.4rem;
                padding: 1rem 0;
            }
        }

        .footer {
            padding: 1.5rem 0;

            span:last-child {
                padding-left: 1.5rem;
            }
        }
    }
}
</style>