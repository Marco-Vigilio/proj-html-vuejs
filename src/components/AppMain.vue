<template>
    <main>
        <div class="contain">

            <DataNumbers />
            <AboutMe />
            <Courses />
            <Shop />
            <Sponsor />
            <Jumbotron />
            <Blog />
        </div>
    </main>
</template>
<script>
import AboutMe from './main/AboutMe.vue';
import DataNumbers from './main/DataNumbers.vue';
import Courses from './main/Courses.vue';
import Shop from './main/Shop.vue';
import Sponsor from './main/Sponsor.vue';
import Jumbotron from './main/Jumbotron.vue';
import Blog from './main/Blog.vue';






export default {
    components: {
        DataNumbers,
        AboutMe,
        Courses,
        Shop,
        Sponsor,
        Jumbotron,
        Blog,
    }
}
</script>
<style lang="scss" scoped>
main {
    div.contain {
        max-width: 1180px;
        margin: 0 auto;
    }
}
</style>