<template>
    <section>
        <span>ABOUT ME</span>
        <div class="introduction">
            <article>
                <h2>How to Be an Alpha Male: The 15 Habits of True Alphas</h2>
            </article>
            <article>
                <p class="questions">Want to learn how to be an alpha male? How to be more masculine? How to be the man
                    you’ve always wanted
                    to be?</p>
                <p class="goals">Your goal is to show the consistency of business, core values, and customer care.
                    Punctuality,
                    responsibility, individuality, accuracy, enthusiasm – you have to clearly explain how these qualities
                    are applicable to your work. And the important thing is you do love what you do.</p>
            </article>
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
    span {
        display: block;
        padding-bottom: 2.5rem;
    }

    .introduction {
        display: flex;

        article {
            width: calc(100% / 2);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;

            h2 {
                font-size: 2.5rem;
                padding-right: 10rem;
            }
        }

        .questions {
            font-size: 1.2rem;
            font-weight: bold;
            padding-bottom: 1rem;
            line-height: 2rem;
        }

        .goals {
            font-size: 1.05rem;
            line-height: 1.5rem;
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