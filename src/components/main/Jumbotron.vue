<template >
    <div class="jumbotron">
        <section>
            <span>REAL STORIES</span>
            <div class="container">
                <p>
                    I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn
                    from the syllabus. Great study portal for people like me.</p>
                <div class="image">
                    <img src="../../assets/img/testimonial-avata-02.jpg" alt="image of Mina Hollace">
                </div>
                <div class="person">
                    <p>Mina Hollace</p>
                    <span>/ Freelancer</span>
                </div>
            </div>
        </section>
        <section id="image_call">
            <img src="../../assets/img/home-movation-testimonial-image.jpg" alt="image call">
        </section>
        <div class="scroll">
            <div><i class="fa-solid fa-caret-up"></i></div>
            <div>1/4</div>
            <div><i class="fa-solid fa-caret-down"></i></div>
        </div>
    </div>
</template>
<script>
export default {
    name: "Jumbotron",
}
</script>
<style lang="scss" scoped>
div.jumbotron {
    background-image: url("../assets/img/background-pattern-wavify.png");
    background-color: gold;
    display: flex;
    position: relative;

    section {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: calc(100% / 2);
        border: 2px solid black;

        .container {
            max-width: 500px;
            background-color: violet;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;

            p {
                text-align: center;
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
        background-color: aqua;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }
}
</style>