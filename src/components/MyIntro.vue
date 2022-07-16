<template>
  <div class="entire_intro">
    <div>AWARD WINNING</div>
    <h2>Pro Barbers</h2>
    <button class="golden_btn">MEET YOUR NEW BARBER</button>
  </div>
</template>

<script>
export default {
  name: 'MyIntro',
};
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
@import '../assets/style/common.scss';
.entire_intro {
  background-image: url('../assets/img/avadabarbers-about-introbackground.jpg');
  object-fit: cover;
  background-position: top;
  background-repeat: no-repeat;
  text-align: center;
  //   todo
  height: 800px;
  div {
    color: $main_color;
  }
  h2 {
    color: $secondary_color;
    font-size: 2rem;
  }
}
</style>
