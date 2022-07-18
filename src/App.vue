<template>
  <div id="app">
    <MyHeader :internalMap="siteSections" />
    <MainComponent />
    <MyFooter :shopInfo="shopLocationInfo" />
  </div>
</template>

<script>
import MainComponent from './components/MainComponent.vue';
import MyHeader from './components/MyHeader.vue';
import MyFooter from './components/MyFooter.vue';

export default {
  name: 'App',
  data() {
    return {
      siteSections: [
        {
          name: 'Introduction',
          id: '#siteintro',
        },
        {
          name: 'Services',
          id: '#siteservices',
        },
        {
          name: 'Shop',
          id: '#siteshop',
        },
        {
          name: 'Featured Product',
          id: '#sitefeatured',
        },
        {
          name: 'Reviews',
          id: '#sitereviews',
        },
        {
          name: 'Blog Posts',
          id: '#siteblog',
        },
        {
          name: 'Footer',
          id: '#sitefooter',
        },
      ],
      shopLocationInfo: [
        'Avada Barbers',
        '123 New York City',
        'New York City',
        'info@yourwebsite.com',
        '+1(555)555-1212',
      ],
    };
  },
  components: {
    MainComponent,
    MyHeader,
    MyFooter,
  },
};
</script>

<style lang="scss">
@import './assets/style/common.scss';
@import './assets/style/variables.scss';
#app {
  margin: 0 auto;
  max-width: 2048px;
  min-width: 880px;
}
</style>
