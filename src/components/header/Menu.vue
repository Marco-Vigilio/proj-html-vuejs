<template>
    <div>
        <div>
            <div class="menu">
                <ul>
                    <li>
                        <a href="#">{{ name }} <i class="fa-solid fa-chevron-down"></i></a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: "Menu",
    props: {
        name: String,
    },
    data() {

    },
}
</script>
<style lang="scss" scoped>
@use '../../style/partilas/variables' as*;

li {
    font-weight: 600;
    margin: 0 1rem;
    border-bottom: 2px solid transparent;
    line-height: normal;
    vertical-align: text-top;

    i {
        font-size: .6rem;

    }

    &:hover {


        a {
            border-bottom: 2px solid $green;
            padding-bottom: .2rem;
            animation-name: slow;
            animation-duration: .3s;
            animation-fill-mode: forwards;

            @keyframes slow {
                0% {
                    color: black;
                }

                100% {
                    color: $green;
                    ;
                }
            }
        }
    }

}
</style>