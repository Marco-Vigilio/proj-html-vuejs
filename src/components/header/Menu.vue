<template>
    <div class="menu">
        <ul>
            <li>
                <a href="#">{{ name }} <i class="fa-solid fa-chevron-down"></i></a>
            </li>
        </ul>
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
li {
    margin: 0 1rem;
    border-bottom: 2px solid transparent;
    line-height: normal;

    vertical-align: text-top;

    i {
        font-size: .6rem;

    }

    &:hover {
        border-bottom: 2px solid black;
    }

}
</style>