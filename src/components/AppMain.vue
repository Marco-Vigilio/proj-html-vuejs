<template>
    <main>
        <div class="contain">
            <DataNumbers />
            <AboutMe />
            <Courses />
            <BookStore />
            <Sponsors />
        </div>
        <Jumbotron />
        <div class="contain">
            <Blogs />
        </div>
    </main>
</template>
<script>
import AboutMe from './main/AboutMe.vue';
import DataNumbers from './main/DataNumbers.vue';
import Courses from './main/Courses.vue';
import BookStore from './main/BookStore.vue';
import Sponsors from './main/Sponsors.vue';
import Jumbotron from './main/Jumbotron.vue';
import Blogs from './main/Blogs.vue';
export default {
    components: {
        DataNumbers,
        AboutMe,
        Courses,
        BookStore,
        Sponsors,
        Jumbotron,
        Blogs,
    }
}
</script>
<style lang="scss" scoped>
main {
    div.contain {
        max-width: 1170px;
        margin: 0 auto;
    }
}
</style>