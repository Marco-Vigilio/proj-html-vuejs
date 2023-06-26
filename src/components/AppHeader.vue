<template>
    <header>
        <nav class="contain">
            <div class="image-logo">
                logo
            </div>
            <div class="nav-bar">
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
                    <li>Social</li>
                </ul>
            </div>
        </nav>

        <div class="jumbotron contain">

        </div>

    </header>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
header {
    background-color: gold;

    nav.contain {
        max-width: 1180px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
    }

    div.nav-bar {
        ul {
            display: flex;

            li {
                margin: 0 1rem;
            }
        }
    }

    div.contain {
        max-width: 1180px;
        margin: 0 auto;
    }
}
</style>