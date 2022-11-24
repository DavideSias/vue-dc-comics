<template>
  <div>
    <header-page />
    <content-page />
    <content-shop-page />
    <footer-page />
  </div>
</template>

<script>
import HeaderPage from '@/components/HeaderPage.vue';
import ContentPage from './components/ContentPage.vue';
import ContentShopPage from './components/ContentShopPage.vue';
import FooterPage from './components/FooterPage.vue';

export default {
  name: 'App',
  components: {
    HeaderPage,
    ContentPage,
    ContentShopPage,
    FooterPage,
  },
};
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
