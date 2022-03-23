<template>
    <div class="grid">
        <img :src="comicImg" alt="">
        <h2>{{ comicSeries.toUpperCase() }}</h2>
    </div>
</template>

<script>

export default {
    name: 'GridShowcaseDC',
    props: {
        comicImg: String,
        comicSeries: String,
    }
}
</script>

<style scoped lang="scss">

.grid{
    flex-basis: calc(100% / 6);
    height: 400px;
    img,
    h2{
        width: 200px;
        padding: 10px;
    }
    h2{
        font-size: 1rem;
    }
}

</style>