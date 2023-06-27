<template>
    <section class="widget">
        <div class="explore">
            <h2>Explore</h2>
            <div class="list">
                <ul>
                    <li v-for="(element, index) in arrayList">
                        {{ index }}
                    </li>
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
</template>
<script>
export default {
    name: "Widget",
    props: {
        arrayList: Array,
    },
    data() {
        return {
            arrayExplore: [],
            arrayInformation: [],
        }
    }
}
</script>
<style lang="scss" scoped>
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
</style>