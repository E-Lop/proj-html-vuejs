<template>
  <main>
    <MyIntro />
    <MyServices />
  </main>
</template>

<script>
import MyIntro from '../components/MyIntro.vue';
import MyServices from '../components/MyServices.vue';
export default {
  name: 'MainComponent',
  components: {
    MyIntro,
    MyServices,
  },
};
</script>

<style lang="scss" scoped></style>
