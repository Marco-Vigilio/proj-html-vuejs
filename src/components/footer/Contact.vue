<template>
    <section class="contact">
        <ul>
            <li>Address</li>
            <li>{{ objectAddress.where }}</li>
            <li>{{ objectAddress.when.number }} ({{ objectAddress.when.hours }}, {{ objectAddress.when.days }})</li>
            <li>{{ objectAddress.email }}</li>
        </ul>
    </section>
</template>
<script>
export default {
    name: "Contact",
    props: {
        objectAddress: Object,
    }
}
</script>
<style lang="scss" scoped></style>