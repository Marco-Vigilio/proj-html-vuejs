<template>
    <div class="jumbotron">
        <section class="spot">
            <div>
                <span>I'm Wingman</span>
                <h1>Peace On Earth A Wonderful Wish But No Way</h1>
                <p>Success isn’t overnight. It’s when everyday you get a little better than the day before. It all adds up.
                </p>
                <button>Get Started For Free <span><i class="fa-solid fa-arrow-right"></i></span></button>
            </div>
        </section>
        <section class="my_image">
            <img class="wingman" src="../../assets/img/home-movation-hero-image.png" alt="image of Wingman">
        </section>

    </div>
</template>
<script>
export default {
    name: "Jumbotron Header",
}
</script>
<style lang="scss" scoped>
@use '../../style/partilas/variables' as*;
@use '../../style/partilas/maxins' as*;

.jumbotron {
    position: relative;
    display: flex;
    padding-top: 3rem;

    .spot {
        width: 50%;
        padding-right: 10rem;
        display: flex;
        align-items: center;

        span {
            text-transform: uppercase;
            @include subTitle;
        }

        p {
            padding-bottom: 1.5rem;
            vertical-align: 60%;
            line-height: 1.8rem;
        }

        button {
            border: none;
            padding: 1rem 2rem;
            border-radius: .3rem;
            background-color: $green;
            color: white;
            @include changeBgColor;

            span {
                margin-left: 1rem;
            }
        }
    }

    .my_image {
        width: 50%;
        padding: 0 1.8rem;
        padding-top: .5rem;
        display: flex;
        justify-content: center;
        align-items: center;

        .wingman {
            z-index: 1;
            width: 100%;
            display: block;
            object-fit: cover;
        }
    }

}
</style>