<template>
    <section>
        <span class="subtitle">BLOG UPDATED</span>
        <h2>Interesting <span class="green">articles updated</span> daily</h2>
        <div class="blogs">
            <Blog v-for="blog in arrayBlog" :image=blog.image :data=blog.data :title=blog.title
                :description="blog.description" />
        </div>
        <div class="link">
            <a href="#" class="green">VIEW ALL POSTS</a>
        </div>

    </section>
</template>
<script>
import Blog from './Blog.vue';
export default {
    name: "Blogs",
    components: {
        Blog
    },
    data() {
        return {
            arrayBlog: [
                {
                    image: "../../../src/assets/img/motivation-blog-04-480x325.jpg",
                    data: "May 13, 2020",
                    title: "How to Stay True to Your Personal Brand",
                    description: "When it comes to your business or career, you want …",
                },
                {
                    image: "../../../src/assets/img/motivation-blog-03-480x325.jpg",
                    data: "May 13, 2020",
                    title: "5 Vital Lessons in 5 Years of Freelancing",
                    description: "Being self-employed and working from home, it’s easy to get …",
                },
                {
                    image: "../../../src/assets/img/motivation-blog-02-480x325.jpg",
                    data: "May 13, 2020",
                    title: "11 Super Useful Tips for Small-Business Owners",
                    description: "Being a small-business owner poses a ton of challenges. We …",
                },
                {
                    image: "../../../src/assets/img/motivation-blog-01-480x325.jpg",
                    data: "May 13, 2020",
                    title: "How to Give Yourself Grace to Start Again",
                    description: "Forgive yourself for bad habits you may have started or …",
                },
            ],
        }
    },
}
</script>
<style lang="scss" scoped>
@use '../../style/partilas/variables' as*;
@use '../../style/partilas/maxins' as*;

.green {
    color: $green;
}

section {
    padding: 4rem 0;

    .subtitle {
        @include subTitle;
    }

    h2 {
        padding: 2rem 0 4rem;
        font-size: 2.4rem;
    }
}

.blogs {
    display: flex;
    display: flex;
    flex-wrap: wrap;
    gap: 2rem;
}

.link {
    display: flex;
    justify-content: center;
    align-items: center;

    a {
        border-bottom: 2px solid $green;

        &:hover {
            border-bottom: 2px solid black;
            color: black
        }
    }
}
</style>