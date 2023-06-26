<template>
    <div class="card">
        <div class="header">immagine</div>
        <div class="main">Descrizione + prezzo</div>
        <div class="footer">N.Lezioni + N.studenti</div>
    </div>

    <div class="card">
        <div class="header">immagine</div>
        <div class="main">Descrizione + prezzo</div>
        <div class="footer">N.Lezioni + N.studenti</div>
    </div>

    <div class="card">
        <div class="header">immagine</div>
        <div class="main">Descrizione + prezzo</div>
        <div class="footer">N.Lezioni + N.studenti</div>
    </div>
</template>
<script>
export default {
    name: "Card",
}
</script>
<style lang="scss" scoped>
.card {
    width: calc(100% / 3);
}
</style>