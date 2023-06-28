<template >
    <div class="jumbotron">
        <section>
            <span class="green">REAL STORIES</span>
            <div class="carousel">
                <p>{{ arrayTestimonial[indexTestimonial].story }}</p>
                <div class="image">
                    <img :src="arrayTestimonial[indexTestimonial].image" alt="">
                </div>
                <div class="person">
                    <p>{{ arrayTestimonial[indexTestimonial].name }}</p>
                    <span>{{ arrayTestimonial[indexTestimonial].work }}</span>
                </div>
            </div>
        </section>
        <section id="image_call">
            <img src="../../assets/img/home-movation-testimonial-image.jpg" alt="image call">
        </section>
        <div class="scroll">
            <div><i class="fa-solid fa-caret-up" @click="previewTestimonial"></i></div>
            <div id="number"><span>{{ index }}</span>/4</div>
            <div><i class="fa-solid fa-caret-down" @click="nextTestimonial"></i></div>
        </div>
    </div>
</template>
<script>
export default {
    name: "Jumbotron",
    data() {
        return {
            indexTestimonial: 0,
            index: "",
            arrayTestimonial: [
                {
                    name: "Mina Hollace",
                    image: "../../../src/assets/img/testimonial-avata-02.jpg",
                    work: "/ Freelancer",
                    story: "I am free to learn at my own pace, follow my own schedule and choose the subject I want to lear from the syllabus. Great study portal for people like me",
                },
                {
                    name: "Madley Pondor",
                    image: "../../../src/assets/img/testimonial-avata-04.jpg",
                    work: "/ IT Specialist",
                    story: "I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.",
                },
                {
                    name: "Luvic Dubble",
                    image: "../../../src/assets/img/testimonial-avata-01.jpg",
                    work: "/ Private Tutor",
                    story: "I am happy with their arrangement of lessons and subjects. They reflect a scientific investigation into effective methods to adopt for learners.",
                },
                {
                    name: "Florence Themes",
                    image: "../../../src/assets/img/testimonial-avata-03.jpg",
                    work: "/ Multimedia Admin",
                    story: "I'm a very strict person so I require everything to be organized and neat. Then, I'll be able to make things right and shine. MaxCoach guys just got me.",
                },
            ],
        }
    },
    methods: {
        previewTestimonial() {
            if (this.indexTestimonial <= 0) {
                this.indexTestimonial = (this.arrayTestimonial.length - 1);
            }
            else {
                this.indexTestimonial--;
            }
        },

        nextTestimonial() {
            if (this.indexTestimonial === (this.arrayTestimonial.length - 1)) {
                this.indexTestimonial = 0;
            }
            else {
                this.indexTestimonial++;
            }
        },
        numberIndex() {
            this.index = this.indexTestimonial + 1;
        },
    },
    mounted() {
        this.numberIndex();
    },
    updated() {
        this.numberIndex();
    },
}
</script>
<style lang="scss" scoped>
@use '../../style/partilas/variables' as*;
@use '../../style/partilas/maxins' as*;

span.green {
    color: $green;
    @include subTitle;
}

div.jumbotron {
    background-image: url("../../../src/assets/img/background-pattern-wavify.png");
    background-color: $backGroundWaves;
    display: flex;
    position: relative;
    padding: 3rem 0;
    margin-bottom: 6rem;

    section {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: calc(100% / 2);

        .carousel {
            max-width: 500px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding-top: 2rem;

            >p {
                text-align: center;
                font-size: 1.6rem;
                font-weight: 600;
                line-height: 3rem;
                padding-bottom: 2rem;
            }

            .image {
                width: 80px;
                height: 80px;
                border-radius: 50%;
                overflow: hidden;

                img {
                    width: 100%;
                }
            }

            .person {
                display: flex;
                flex-direction: column;
                align-items: center;

                padding-top: 2rem;

                p {
                    font-size: 1.2rem;
                    font-weight: 600;
                    letter-spacing: .1rem;
                    padding-bottom: 1rem;
                }

                span {
                    font-size: .9rem;
                }
            }
        }
    }

    #image_call {
        img {
            width: 100%;
        }
    }

    .scroll {
        width: 100px;
        height: 100px;
        border-radius: 50%;
        display: flex;
        align-items: center;
        flex-direction: column;
        justify-content: center;
        background-color: white;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);

        #number {
            font-weight: 600;
            letter-spacing: .1rem;
        }

        i {
            font-size: 1.2rem;
            color: #d5d5d5;
        }
    }
}
</style>