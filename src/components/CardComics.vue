<template lang="">
    <div>
        <div class="img-container">
            <img :src="comicsInfo.thumb" alt="">
        </div>
        <h2>
            {{comicsInfo.series.toUpperCase()}}
        </h2>
    </div>
</template>
<script>
export default {
    name: "CardComics",
    props: [
        "comicsInfo",
    ]
}
</script>
<style lang="scss">
    @use "../styles/general.scss";
</style>