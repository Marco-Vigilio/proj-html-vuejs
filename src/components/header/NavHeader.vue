<template>
    <nav>
        <div class="image_logo">
            <img src="../../assets/img/dark-logo.png" alt="">
        </div>


        <div class="menu">
            <ul>
                <Menu v-for="element in arrayMenu" :name=element.name />
            </ul>
        </div>

        <div class="social">
            <ul>
                <li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
                <li><a href="#"><i class="fa-brands fa-facebook-f"></i></a></li>
                <li><a href="#"><i class="fa-brands fa-instagram"></i></a></li>
                <li><a href="#"><i class="fa-brands fa-linkedin"></i></a></li>
            </ul>
        </div>
    </nav>
</template>
<script>
import Menu from './Menu.vue';
export default {
    name: "Nav Header",
    components: {
        Menu
    },
    data() {
        return {
            arrayMenu: [
                {
                    name: "Home"
                },
                {
                    name: "Pages"
                },
                {
                    name: "Courses"
                },
                {
                    name: "Features"
                },
                {
                    name: "Blog"
                },
                {
                    name: "Shop"
                },

            ]
        }
    }
}
</script>
<style lang="scss" scoped>
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.5rem 0;

    .menu {
        ul {
            display: flex;
        }
    }

    .image_logo {
        width: 160px;

        img {
            width: 100%;
        }
    }

    .social {
        display: flex;
        justify-content: flex-end;

        ul {
            display: flex;

            li {
                padding-left: 1.5rem;

                i {
                    font-size: 1.1rem;
                }
            }
        }
    }
}
</style>