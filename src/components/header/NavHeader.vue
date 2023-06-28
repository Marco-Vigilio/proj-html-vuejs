<template>
    <nav>
        <div class="image_logo">
            <img src="../../assets/img/dark-logo.png" alt="Logo MaxChoach">
        </div>


        <div class="menu">
            <ul>
                <Menu v-for="element in arrayMenu" :name=element.name />
            </ul>
        </div>

        <div class="social">
            <ul>
                <li><a href="#"><i class="fa-brands fa-twitter"></i></a>
                    <div>twitter</div>
                </li>
                <li><a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                    <div>facebook</div>
                </li>
                <li><a href="#"><i class="fa-brands fa-instagram"></i></a>
                    <div>instagram</div>
                </li>
                <li><a href="#"><i class="fa-brands fa-linkedin"></i></a>
                    <div>linkedin</div>
                </li>
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
@use '../../style/partilas/variables' as*;
@use '../../style/partilas/maxins' as*;

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
                position: relative;
                padding-left: 1.5rem;

                a {

                    i {
                        font-size: 1.1rem;
                        @include changeBgColorGreen;
                    }
                }

                div {
                    display: none;
                    position: absolute;
                    right: 0;
                    font-weight: 600;
                    padding: .5rem;
                    margin-top: .5rem;
                    background-color: black;
                    color: white;
                    border-radius: .3rem;
                }

                a:hover+div {

                    display: block;
                }
            }


        }
    }
}
</style>