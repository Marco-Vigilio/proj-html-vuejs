<template>
    <section>
        <div class="about_store">
            <span class="subtitle">BOOK STORE ONLINE</span>
            <h2>Be Alpha With <span class="green">Wingman's Book</span></h2>
            <ul>
                <li><span class="green"><i class="fa-solid fa-check"></i></span>Help you understand yourself better</li>
                <li><span class="green"><i class="fa-solid fa-check"></i></span>Revealing mature tips</li>
                <li><span class="green"><i class="fa-solid fa-check"></i></span>Give the right advice</li>
                <li><span class="green"><i class="fa-solid fa-check"></i></span>Fascinating examples of alpha man</li>
            </ul>
            <button>
                <link rel="stylesheet" href="#"> Get Free Ebook
            </button>
        </div>
        <div class="books">
            <div class="book">
                <div class="image_book">
                    <img src="../../assets/img/product-book-11-400x400.jpg" alt="image of my book">
                </div>
                <div class="info">
                    <p><a href="#">Alpha man by Maxcoach</a></p>
                    <span class="big_num green">29</span><span class="green">.00</span><span
                        class="big_num green">&dollar;</span>
                </div>
            </div>
            <div class="book">
                <div class="image_book">
                    <img src="../../assets/img/product-book-10-400x400.jpg" alt="image of my book">
                </div>
                <div class="info">
                    <p><a href="#">Real man 4.0 by Maxcoach</a></p>
                    <span class="big_num green">39</span><span class="green">.00</span><span
                        class="big_num green">&dollar;</span>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    name: "Book Store",
    data() {
        return {
            books: [
                {
                    title: "Alpha man by Maxcoach",
                    image: "../../../src/assets/img/product-book-11-400x400.jpg",
                    price: ["29", "00"],
                },
                {
                    title: "Real man 4.0 by Maxcoach",
                    image: "../../../src/assets/img/product-book-10-400x400.jpg",
                    price: ["39", "00"],
                },
            ],
        }
    }
}
</script>
<style lang="scss" scoped>
@use '../../style/partilas/variables' as*;
@use '../../style/partilas/maxins' as*;

span.green {
    color: $green;
}

section {
    display: flex;
    padding: 2rem 0 1rem;

    span.subtitle {
        display: block;
        @include subTitle;
    }

    .about_store {
        width: 40%;

        h2 {
            font-size: 2.5rem;
            padding: 2rem 1rem 2rem 0;
        }

        ul {
            li {
                padding-bottom: 1rem;

                i {
                    padding-right: 1rem;
                    font-size: 1.2rem;
                }
            }
        }

        button {
            display: flex;
            justify-content: center;
            border: none;
            margin-top: 1rem;
            padding: 1rem 4rem;
            border-radius: 0.3rem;
            background-color: $green;
            color: white;
            @include changeBgColor;
        }
    }

    .books {
        width: calc(100% - 40%);
        display: flex;

        .book:first-child {
            margin: 0 2rem;
        }

        .book .image_book img {
            transition: 1s;
        }

        .book:hover .image_book img {
            transform: scale(1.1);
        }

        .book {
            width: calc(100% / 2);

            .image_book {
                width: 100%;
                overflow: hidden;

                img {
                    width: 100%;
                    display: block;
                }
            }

            .info {
                text-align: center;

                p {
                    font-size: 1.4rem;
                    padding: 1rem 0;
                    font-weight: bold;

                    a {
                        @include changeBgColorGreen;
                    }
                }

                span {
                    font-weight: 600;
                }
            }

            .big_num {
                font-size: 1.5rem;
            }
        }
    }
}
</style>