<template>
    <section class="contact">
        <h2>Address</h2>
        <ul class="list">
            <li>{{ objectAddress.where }}</li>
            <li>{{ objectAddress.when.number }} ({{ objectAddress.when.hours }}, {{ objectAddress.when.days }})</li>
            <li id="email"><a href="#">{{ objectAddress.email }}</a></li>
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
@use '../../style/partilas/variables' as*;
@use '../../style/partilas/maxins' as*;

.contact {
    display: flex;
    flex-direction: column;

    h2 {
        @include subTitleFooter;
    }

    .list li {
        line-height: 2.3rem;
        padding-top: .5rem;
        color: $gray;
    }

    #email {
        a {
            color: $gray;
            @include changeBgColorGreen;
        }

    }

    .social {
        display: flex;
        margin-top: 1rem;

        i {
            font-size: 1.5rem;
            margin-right: 1.8rem;
            color: $gray;
            transition: .3s;

            &:hover {
                color: white;
            }
        }
    }
}
</style>