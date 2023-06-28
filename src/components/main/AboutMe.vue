<template>
    <section>
        <span class="section green">ABOUT ME</span>
        <div class="introduction">
            <article>
                <h2>How to Be an Alpha Male: The 15 Habits of True Alphas</h2>
            </article>
            <article>
                <p class="questions">Want to learn how to be <span class="green">an alpha male</span>? How to be more
                    masculine? How to be the man
                    you’ve always wanted
                    to be?</p>
                <p class="goals">Your goal is to show the consistency of business, core values, and customer care.
                    Punctuality,
                    responsibility, individuality, accuracy, enthusiasm – you have to clearly explain how these qualities
                    are applicable to your work. And the important thing is you do love what you do.</p>
            </article>
        </div>
        <div class="about">
            <article class="video">
                <a href="#">
                    <img id="video_youtube" src="../../assets/img/home-movation-video-poster-670x450.jpg"
                        alt="image video of Theme Move">
                    <img class="youtube_icon" src="../../assets/img/icon-youtube-play.png" alt="image icon Youtube">
                </a>
            </article>
            <article class="cit">
                <div>
                    <h3>"Every morning you have two choices: continue to sleep with your dreams, or wake up and chase them."
                    </h3>
                </div>
                <div>
                    <img src="../../assets/img/home-movation-shape-01.png" alt="lazy">
                    <span class="name">Kaixa Stark</span>
                    <span>WINGMAN</span>
                </div>
            </article>
        </div>
    </section>
</template>
<script>
export default {
    name: "About Me",
}
</script>
<style lang="scss" scoped>
@use '../../style/partilas/variables' as*;
@use '../../style/partilas/maxins' as*;

span.green {
    color: $green;
}

section {
    span.section {
        display: block;
        padding: 2rem 0 .5rem;
        font-weight: 600;
        letter-spacing: .1rem;

    }

    .introduction {
        display: flex;

        article {
            width: calc(100% / 2);
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            overflow: hidden;

            h2 {
                font-size: 2.5rem;
                padding-right: 10rem;
            }
        }

        .questions {
            font-size: 1.1rem;
            font-weight: bold;
            padding-bottom: 1rem;
            line-height: 2rem;
        }

        .goals {
            font-size: .95rem;
            line-height: 1.6rem;
        }
    }

    .about {
        display: flex;
        padding: 3rem 0;

        article.video {
            position: relative;
            display: flex;
            width: 57%;
            border-radius: .4rem;
            overflow: hidden;

            #video_youtube {
                @include scale;
            }

            img {
                width: 100%;
                display: block;
            }

            .youtube_icon {
                position: absolute;
                width: 90px;
                top: 50%;
                left: 50%;
                transform: translate(-50%, -50%);
            }
        }

        article.cit {
            display: flex;
            flex-direction: column;
            justify-content: center;
            width: calc(100% - 57%);
            padding-left: 5rem;

            :first-child {
                h3 {
                    font-size: 1.8rem;
                    padding-bottom: 3rem;
                    line-height: 3rem;
                }
            }

            :last-child {
                display: flex;
                flex-direction: column;

                img {
                    width: 30px;
                }

                span.name {
                    font-size: 1.4rem;
                    padding: 1.5rem 0rem 1rem;
                    font-weight: bold;
                }
            }
        }

        //no margin, PADDING
    }
}
</style>