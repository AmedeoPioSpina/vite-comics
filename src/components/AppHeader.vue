<template lang="">
    <header>
        <section class="nav-container">
            <nav>
                <div class="logo-container">
                    <img src="../assets/img/dc-logo.png" alt="">
                </div>
                <ul class="nav-links-container">
                    <li v-for="(item, index) in navLinksNamesList" :class="index == activeIndex ? active : no-active">
                        {{
                            item
                        }}
                    </li>
                </ul>
            </nav>
        </section>
    </header>
</template>

<script>
export default {
    name: "AppHeader",
    data() {
        return {
            navLinksNamesList: [
                "CHARACTERS",
                "COMICS",
                "MOVIES",
                "TV",
                "GAMES",
                "COLLECTIBLES",
                "VIDEOS",
                "FANS",
                "NEWS",
                "SHOP"
            ],
            activeIndex: 1,
        }
    }
}
</script>

<style lang="scss">
    @use '../styles/general.scss' as *;
</style>