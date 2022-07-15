<template>
  <div id="app">
    <MyHeader :internalMap="siteSections" />
    <MainComponent />
  </div>
</template>

<script>
import MainComponent from './components/MainComponent.vue';
import MyHeader from './components/MyHeader.vue';

export default {
  name: 'App',
  data() {
    return {
      siteSections: [
        {
          name: 'Introduction',
          id: '#intro',
        },
        {
          name: 'Services',
          id: '#services',
        },
        {
          name: 'Shop',
          id: '#shop',
        },
        {
          name: 'Featured Product',
          id: '#featured',
        },
        {
          name: 'Reviews',
          id: '#reviews',
        },
        {
          name: 'Blog Posts',
          id: '#blog',
        },
        {
          name: 'Footer',
          id: '#footer',
        },
      ],
    };
  },
  components: {
    MainComponent,
    MyHeader,
  },
};
</script>

<style lang="scss">
@import './assets/style/common.scss';
@import './assets/style/variables.scss';
</style>
