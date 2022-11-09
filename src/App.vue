<script>
import AppHeader from "../src/components/AppHeader.vue";
import ComicsList from "../src/components/ComicsList.vue";
import AppIcons from "../src/components/AppIcons.vue";

export default {
  components: {
    AppHeader,
    ComicsList,
    AppIcons
  }
}
</script>

<template>
<AppHeader />

<ComicsList />

<AppIcons />
</template>

<style lang="scss">
@use "../src/styles/general.scss";
</style>
