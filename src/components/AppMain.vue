<template lang="">
    <main>
        <section>
            <div class="main-background-image">

            </div>
            <div class="main-content-container">
                <CardsContainer />
            </div>
        </section>
    </main>
</template>
<script>
import CardsContainer from './CardsContainer.vue';

export default {
    name: "AppMain",
    components: {
        CardsContainer
    },
    data() {
        return {

        }
    }
}
</script>
<style lang="scss">
    @use "../styles/general.scss" as *;
</style>