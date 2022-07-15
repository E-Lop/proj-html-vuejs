<template>
  <div id="app">
    <MyHeader />
    <MainComponent />
  </div>
</template>

<script>
import MainComponent from './components/MainComponent.vue';
import MyHeader from './components/MyHeader.vue';

export default {
  name: 'App',
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
