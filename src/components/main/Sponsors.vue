<template>
    <div class="sponsors">
        <div class="sponsor">
            <img src="../../assets/img/client-logo-05-primary.png" alt="image of Its Alive!">
        </div>
        <div class="sponsor">
            <img src="../../assets/img/client-logo-06-primary.png" alt="image of Its Alive!">
        </div>
        <div class="sponsor">
            <img src="../../assets/img/client-logo-07-primary.png" alt="image of Its Alive!">
        </div>
        <div class="sponsor">
            <img src="../../assets/img/client-logo-04-primary.png" alt="image of Its Alive!">
        </div>
        <div class="sponsor">
            <img src="../../assets/img/client-logo-03-primary.png" alt="image of Its Alive!">
        </div>
        <div class="sponsor">
            <img src="../../assets/img/client-logo-02-primary.png" alt="image of Its Alive!">
        </div>
    </div>
</template>
<script>
export default {
    name: "Sponsor",
}
</script>
<style lang="scss" scoped>
.sponsors {
    display: flex;
    justify-content: space-between;
    padding: 7rem 0;

    div.sponsor {
        width: calc(100% / 6);
        height: 70px;
        display: flex;
        justify-content: center;

        img {
            width: 60%;
            object-fit: contain;
            filter: grayscale(70%);
            opacity: 40%;
            transition: .4s;

            &:hover {
                filter: grayscale(0%);
                opacity: 100%;
            }
        }
    }
}
</style>