<template>
    <section class="widget">
        <div class="explore">
            <h2>Explore</h2>
            <div class="list">
                <ul>
                    <li v-for="(element, index) in arrayExplore1">
                        {{ element }}
                    </li>
                </ul>
                <ul>
                    <li v-for="(element, index) in arrayExplore2">
                        {{ element }}
                    </li>
                </ul>
            </div>
        </div>
        <div class="information">
            <h2>information</h2>
            <ul>
                <li v-for="(element, index) in arrayInformation">
                    {{ element }}
                </li>
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
            arrayExplore1: [],
            arrayExplore2: [],
            arrayInformation: [],
        }
    },
    methods: {
        fillArray() {
            this.arrayExplore1 = (this.arrayList.slice(0, 3)); //inizia da 0 e prende 3 elementi
            this.arrayExplore2 = (this.arrayList.slice(3, 6));
            this.arrayInformation = (this.arrayList.slice(6, this.arrayList.length));
            /*
            for (let index = 0; index < 3; index++) {
                this.arrayExplore1 = this.arrayList[index];
            }

            for (let index = 3; index < 6; index++) {
                this.arrayExplore2 = this.arrayList[index];
            }
            for (let index = 6; index < this.arrayList.length; index++) {
                this.arrayInformation = this.arrayList[index];
            }
            */
        }
    },
    mounted() {
        this.fillArray();
    },
}
</script>
<style lang="scss" scoped>
.widget {
    .explore {
        div.list {
            display: flex;

            ul {
                width: calc(100% / 2);
                padding-top: .5rem;

                li {
                    line-height: 2.3rem;
                }
            }
        }
    }

    .explore,
    .information {
        width: calc(100% / 2);

        ul {
            padding-top: .5rem;

            li {
                line-height: 2.3rem;
            }
        }
    }
}
</style>