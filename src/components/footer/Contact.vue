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

.contact {
    display: flex;
    flex-direction: column;

    .list li {
        line-height: 2.3rem;
        padding-top: .5rem;
        color: $gray;
    }

    #email {
        a {
            color: $gray;

            &:hover {
                animation-name: slowEmail;
                animation-duration: .3s;
                animation-fill-mode: forwards;

                @keyframes slowEmail {
                    0% {
                        color: $gray;
                    }

                    100% {
                        color: $green;
                    }
                }
            }
        }

    }

    .social {
        display: flex;
        margin-top: 1rem;

        i {
            font-size: 1.5rem;
            margin-right: 1.8rem;
            color: $gray;

            &:hover {
                animation-name: slow;
                animation-duration: .3s;
                animation-fill-mode: forwards;

                @keyframes slow {
                    0% {
                        color: $gray;
                    }

                    100% {
                        color: white;
                        ;
                        ;
                    }
                }
            }
        }
    }
}
</style>