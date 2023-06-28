<template>
    <div class="blog">
        <a href="#">
            <div class="image">
                <img :src="image" alt="image of work">
            </div>
        </a>
        <div class="info_blog">
            <span class="when"><i class="fa-regular fa-calendar"></i> {{ data }}</span>
            <p><a href="#">{{ title }}</a></p>
            <span>{{ description }}</span>
        </div>
    </div>
</template>
<script>
export default {
    props: {
        image: String,
        data: String,
        title: String,
        description: String,
    },
}
</script>
<style lang="scss" scoped>
@use '../../style/partilas/variables' as*;
@use '../../style/partilas/maxins' as*;

.blog img {
    transition: 1s;
}

.blog:hover img {
    transform: scale(1.1);
}

.blog {
    width: (calc((100% - 8rem) / 4));

    .image {
        width: 100%;
        border-radius: .6rem;
        overflow: hidden;

        img {
            width: 100%;
            display: block;
        }
    }

    .info_blog {
        padding: 1.5rem 0 2rem;

        span.when {
            color: gray;
            font-size: .9rem;
        }

        p {
            font-size: 1.3rem;
            padding: 1rem 0;
            line-height: 2rem;
            font-weight: 600;

            a {
                transition: .4s;

                &:hover {
                    color: $green;
                }
            }
        }
    }
}
</style>