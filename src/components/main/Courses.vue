<template>
    <section>
        <div class="title">
            <span class="subtitle">BEGIN YOUR JOURNEY AT MAXCOACH</span>
            <h2>Latest <span class="green">Online Courses</span></h2>
        </div>
        <div class="cards">
            <Card v-for="course in arrayCourses" :name=course.name :image=course.image :numLesson=course.numberLesson
                :numStudents=course.students :priceNumber=course.price[0] :priceNumberDecimal=course.price[1] />
        </div>
        <div class="button">
            <button class="button">View all courses<span><i class="fa-solid fa-arrow-right"></i></span></button>
        </div>
    </section>
</template>
<script>
import Card from './Card.vue';
export default {
    name: "Courses",
    components: {
        Card,
    },
    data() {
        return {
            arrayCourses: [
                {
                    name: "How to be Successful: Create A Growth Mindset For Success",
                    numberLesson: 3,
                    students: 50,
                    price: ["30", "00"],
                    image: "../../../src/assets/img/motivation-course-06-480x298.jpg",
                },
                {
                    name: "How to Build Confidence in Your Abilities",
                    numberLesson: 1,
                    students: 50,
                    price: ["30", "00"],
                    image: "../../../src/assets/img/motivation-course-05-480x298.jpg",
                },
                {
                    name: "Productivity Machine – Focus in a Distracted World",
                    numberLesson: 5,
                    students: 50,
                    price: ["20", "00"],
                    image: "../../../src/assets/img/motivation-course-04-480x298.jpg",
                },
                {
                    name: "Effective Time Management Mastery – Complete Guide",
                    numberLesson: 18,
                    students: 50,
                    price: ["20", "00"],
                    image: "../../../src/assets/img/motivation-course-03-480x298.jpg",
                },
                {
                    name: "Body Language Secrets for Entrepreneurs",
                    numberLesson: 19,
                    students: 50,
                    price: ["25", "99"],
                    image: "../../../src/assets/img/motivation-course-02-480x298.jpg",
                },
                {
                    name: "Management Skills: The Science of Leadership",
                    numberLesson: 17,
                    students: 50,
                    price: ["19", "99"],
                    image: "../../../src/assets/img/motivation-course-01-480x298.jpg",
                },
            ],
        }
    },
}
</script>
<style lang="scss" scoped>
@use '../../style/partilas/variables' as*;
@use '../../style/partilas/maxins' as*;

span.green {
    color: $green;
}

section {
    padding: 6rem 0 3rem;

    div.title {
        text-align: center;
        padding-bottom: 2rem;

        span.subtitle {
            @include subTitle;
            color: $gray;
        }

        h2 {
            font-size: 2.5rem;
            padding: 2rem 0;
        }
    }

    .cards {
        display: flex;
        flex-wrap: wrap;
        gap: 2rem;
    }

    .button {
        display: flex;
        justify-content: center;
        border: none;
        margin: 1rem 0 .5rem;
        padding: 1rem 4rem;
        border-radius: .3rem;

        button {
            background-color: $green;
            color: white;
            @include changeBgColor;

            span {
                margin-left: 1rem;
            }
        }

    }
}
</style>