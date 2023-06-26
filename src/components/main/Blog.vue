<template>
    <div class="blog">
        <div class="image">
            <img :src="image" alt="image of work">
        </div>
        <div class="info_blog">
            <span><i class="fa-regular fa-calendar"></i> {{ data }}</span>
            <p>{{ title }}</p>
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
.blog {
    width: (calc((100% - 4rem) / 4));

    .image {
        width: 100%;
        border-radius: .6rem;
        overflow: hidden;

        img {
            width: 100%;
        }
    }

    .info_blog {
        padding: 1.5rem 0 2rem;

        p {
            font-size: 1.4rem;
            padding: 1rem 0;
            line-height: 2rem;
        }

        span {
            font-size: 1rem;
        }
    }
}
</style>