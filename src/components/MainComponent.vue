<template>
  <main>
    <MyIntro />
    <MyServices />
    <MyShop />
    <MyFeatured />
    <MyReviews />
  </main>
</template>

<script>
import MyIntro from '../components/MyIntro.vue';
import MyServices from '../components/MyServices.vue';
import MyShop from '../components/MyShop.vue';
import MyFeatured from '../components/MyFeatured.vue';
import MyReviews from '../components/MyReviews.vue';
export default {
  name: 'MainComponent',
  components: {
    MyIntro,
    MyServices,
    MyShop,
    MyFeatured,
    MyReviews,
  },
};
</script>

<style lang="scss" scoped></style>
