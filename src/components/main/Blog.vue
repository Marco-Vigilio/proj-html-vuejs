<template>
    <section>
        <span>Titilino</span>
        <h1>Titolo</h1>
        <div class="items">
            <div>Item</div>
            <div>Item</div>
            <div>Item</div>
            <div>Item</div>
        </div>
        <a href="#">Blogs</a>
    </section>
</template>
<script>
export default {
    name: "Blog",
}
</script>
<style lang="scss" scoped>
.items {
    display: flex;
    justify-content: space-between;
}

a {
    display: flex;
    justify-content: center;
}
</style>