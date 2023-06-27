<template>
    <footer>
        <div class="contain">
            <div class="flex">
                <Contact :objectAddress="objectContact" />
                <Widget :arrayList="arrayWidget" />
            </div>
            <p>© 2020 Maxcoach. All Rights Reserved</p>
        </div>
    </footer>
</template>
<script>
import Contact from "./footer/Contact.vue";
import Widget from "./footer/Widget.vue";
export default {
    components: {
        Contact,
        Widget,
    },
    data() {
        return {
            objectContact: {
                where: "382 NE 191st St # 87394 Miami, FL 33179-3899",
                when: {
                    number: "+1 (305) 547-9909",
                    hours: "9am - 5pm EST",
                    days: "Monday - Friday",
                },
                email: "support@maxcoach.com",
            },

            arrayWidget: [
                "Start here",
                "Blog",
                "About us",
                "Success story",
                "Courses",
                "Contact us",
                "Membership",
                "Purchase guide",
                "Privacy policy",
                "Terms of service",
            ]
        }
    },
}
</script>
<style lang="scss" scoped>
@use '../style/partilas/variables' as*;

footer {
    background-color: #3F3A64;
    color: white;

    div.contain {
        max-width: 1170px;
        margin: 0 auto;

        .flex {
            display: flex;
            padding: 3rem 0 4rem;

            section {
                width: calc(100% / 2);
                display: flex;
            }
        }

        p {
            text-align: center;
            padding: 1rem 0 3rem;
            color: $gray;
        }
    }
}
</style>