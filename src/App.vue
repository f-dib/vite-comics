<script>
import AppNav from './components/header/AppNav.vue';
import AppContent from './components/main/AppContent.vue';
import InfoBar from './components/main/InfoBar.vue';
import FooterLink from './components/footer/FooterLink.vue';
import FooterSocial from './components/footer/FooterSocial.vue';

export default {
  components: {
    AppNav,
    AppContent,
    InfoBar,
    FooterLink,
    FooterSocial
  }
}
</script>


<template>
    <AppNav></AppNav>
    <AppContent></AppContent>
    <InfoBar></InfoBar>
    <FooterLink></FooterLink>
    <FooterSocial></FooterSocial>
</template>


<style lang="scss">
  @use './style/general.css' as *;
</style>
