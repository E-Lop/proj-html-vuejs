<template>
  <main>
    <MyIntro />
    <MyServices />
    <MyShop />
    <MyFeatured />
  </main>
</template>

<script>
import MyIntro from '../components/MyIntro.vue';
import MyServices from '../components/MyServices.vue';
import MyShop from '../components/MyShop.vue';
import MyFeatured from '../components/MyFeatured.vue';
export default {
  name: 'MainComponent',
  components: {
    MyIntro,
    MyServices,
    MyShop,
    MyFeatured,
  },
};
</script>

<style lang="scss" scoped></style>
