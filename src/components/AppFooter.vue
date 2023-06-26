<template>
    <footer>
        <div class="contain">
            <div class="flex">
                <section class="contact">
                    <ul>
                        <li>Contatti</li>
                    </ul>
                </section>
                <section class="widget">
                    <div class="explore">
                        <h2>Explore</h2>
                        <div class="list">
                            <ul>
                                <li>Qualcosa</li>
                            </ul>
                            <ul>
                                <li>Qualcosa</li>
                            </ul>
                        </div>
                    </div>
                    <div class="information">
                        <h2>information</h2>
                        <ul>
                            <li>Qualcosa</li>
                        </ul>
                    </div>
                </section>
            </div>
            <p>Copywrite</p>
        </div>
    </footer>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
footer {
    background-color: rgb(72, 72, 72);

    div.contain {
        max-width: 1170px;
        margin: 0 auto;

        .flex {
            display: flex;

            section {
                background-color: red;
                width: calc(100% / 2);
                display: flex;
            }

            .widget {
                .explore {
                    div.list {
                        display: flex;

                        ul {
                            width: calc(100% / 2);
                        }
                    }
                }

                .explore,
                .information {
                    width: calc(100% / 2);
                }
            }
        }

        p {
            text-align: center;
        }
    }
}
</style>