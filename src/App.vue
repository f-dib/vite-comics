<script>
import AppNav from './components/header/AppNav.vue';
import AppContent from './components/main/AppContent.vue';
import FooterLink from './components/footer/FooterLink.vue';

export default {
    components: {
      AppNav,
      AppContent,
      FooterLink
    }
}
</script>


<template>
    <AppNav></AppNav>
    <AppContent></AppContent>
    <FooterLink></FooterLink>
</template>


<style lang="scss">
  @use './style/general.css' as *;
</style>
