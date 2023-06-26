<template>
    <nav>
        <div class="image-logo">
            logo
        </div>

        <div class="menu">
            <ul>
                <li>qualcosa</li>
                <li>qualcosa</li>
                <li>qualcosa</li>
                <li>qualcosa</li>
                <li>qualcosa</li>
                <li>qualcosa</li>
            </ul>
        </div>

        <div class="social">
            <ul>
                <li>icone</li>
            </ul>
        </div>
    </nav>
</template>
<script>
export default {
    name: "Nav Header",

}
</script>
<style lang="scss" scoped>
nav {
    display: flex;
    justify-content: space-between;

    .menu {

        ul {
            display: flex;

            li {
                margin: 0 1rem;
            }
        }
    }

    .social {
        background-color: violet;
        display: flex;
        justify-content: flex-end;
    }
}
</style>