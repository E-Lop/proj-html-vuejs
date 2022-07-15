<template>
  <div id="app">
    <MainComponent />
  </div>
</template>

<script>
import 'bootstrap';
import 'bootstrap/dist/css/bootstrap.min.css';
import MainComponent from './components/MainComponent.vue';

export default {
  name: 'App',
  components: {
    MainComponent,
  },
};
</script>

<style lang="scss">
@import './assets/style/common.scss';
</style>
