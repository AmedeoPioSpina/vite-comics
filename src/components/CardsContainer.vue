<template lang="">
    <div class="sez-title">
        CURRENT SERIES
    </div>
    <div class="cards-container">
        <CardComics v-for="item in cardsList"
        :comicsInfo="item" />
    </div>
</template>
<script>
import axios from "axios";
import cards from "../assets/json/dc-comics.json";
import CardComics from "./CardComics.vue";

export default {
    name: "CardsContainer",
    components: {
        CardComics
    },
    data() {
        return {
            cardsList: cards,
        }
    },
    methods: {

    }

}
</script>
<style lang="scss">
    @use "../styles/general.scss"
</style>