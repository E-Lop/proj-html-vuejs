<template>
  <main>
    <MyIntro />
    <MyServices />
    <MyShop />
  </main>
</template>

<script>
import MyIntro from '../components/MyIntro.vue';
import MyServices from '../components/MyServices.vue';
import MyShop from '../components/MyShop.vue';
export default {
  name: 'MainComponent',
  components: {
    MyIntro,
    MyServices,
    MyShop,
  },
};
</script>

<style lang="scss" scoped></style>
