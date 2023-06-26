<template>
    <header>
        <div class="contain">
            <nav>
                <div class="image-logo">
                    logo
                </div>

                <div class="icons">
                    <ul>
                        <li>icone</li>
                    </ul>
                </div>
            </nav>

            <div class="jumbotron">
                <div class="spot">
                    qualcosa
                </div>
                <div class="my_image">
                    immagine
                </div>
            </div>
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

    div.contain {
        max-width: 1180px;
        margin: 0 auto;

        nav {
            display: flex;
            justify-content: space-between;

            .icons {
                background-color: violet;
                display: flex;
                justify-content: flex-end;
            }
        }

        .jumbotron {
            display: flex;

            div.my_image,
            div.spot {
                width: calc(100% / 2);
                height: 300px;
            }

            .spot {
                background-color: red;
                border: 2px solid black;
            }

            .my_image {
                background-color: green;
                border: 2px solid black;
            }

        }
    }


}
</style>