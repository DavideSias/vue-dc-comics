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
@import url('https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@300;400;700&display=swap');

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html{
  font-family: 'Roboto Condensed', sans-serif;
}
</style>
