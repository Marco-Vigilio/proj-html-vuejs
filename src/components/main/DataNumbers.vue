<template>
    <div class="numbers">
        <div class="data">numeri</div>
        <div class="data">numeri</div>
        <div class="data">numeri</div>
        <div class="data">numeri</div>
    </div>
</template>
<script>
export default {
    name: "Data Numbers",
}
</script>
<style lang="scss" scoped>
div.numbers {
    display: flex;
    justify-content: space-between;

    div.data {
        width: calc(100% / 4);
        background-color: blue;
        border: 2px solid black;
        display: flex;
        justify-content: center;
    }
}
</style>