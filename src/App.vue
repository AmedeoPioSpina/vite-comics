<template lang="">
  <AppHeader />
  <!-- <AppMain/>
  <AppFooter/> -->
</template>

<script>
  import AppHeader from "./components/Appheader.vue";

  export default {
    components: {
      AppHeader,
    }
  }
</script>

<style lang="scss" scoped>
  @use './styles/general.scss' as *;
</style>