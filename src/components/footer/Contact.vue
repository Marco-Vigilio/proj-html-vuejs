<template>
    <section class="contact">
        <h2>Address</h2>
        <ul class="list">
            <li>{{ objectAddress.where }}</li>
            <li>{{ objectAddress.when.number }} ({{ objectAddress.when.hours }}, {{ objectAddress.when.days }})</li>
            <li>{{ objectAddress.email }}</li>
            <li>
                <ul class="social">
                    <li><a href="#"><i class="fa-brands fa-square-facebook"></i></a></li>
                    <li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
                    <li><a href="#"><i class="fa-brands fa-instagram"></i></a></li>
                    <li><a href="#"><i class="fa-brands fa-linkedin"></i></a></li>
                </ul>
            </li>
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
<style lang="scss" scoped>
.contact {
    display: flex;
    flex-direction: column;

    .list li {
        line-height: 2.3rem;
        padding-top: .5rem;
    }

    .social {
        display: flex;
        margin-top: 1rem;

        i {
            font-size: 1.5rem;
            margin-right: 1.8rem;
        }
    }
}
</style>