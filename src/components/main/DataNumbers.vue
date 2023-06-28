<template>
    <div class="numbers">
        <div class="data">
            <span>1.926</span>
            <p>FINISHED SESSIONS</p>
        </div>
        <div class="data">
            <span>100%</span>
            <p>SATISFACTION RATE</p>
        </div>
        <div class="data">
            <span>3092+</span>
            <p>ENROLLED LEARNERS</p>
        </div>
        <div class="data">
            <span>200</span>
            <p>ONLINE INSTRUCTORS</p>
        </div>
    </div>
</template>
<script>
export default {
    name: "Data Numbers",
}
</script>
<style lang="scss" scoped>
@use '../../style/partilas/variables' as*;

div.numbers {
    display: flex;
    justify-content: space-between;
    background-image: url("../../assets/img/background-pattern-grid-line-06.png");
    margin: 6rem 0;

    div.data {
        width: calc(100% / 4);
        padding: 1rem;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;

        span {
            font-size: 2.5rem;
            padding-bottom: .5rem;
            color: $green;
            font-weight: 900;
        }

        p {
            font-weight: 600;
            letter-spacing: .1rem;
        }
    }
}
</style>