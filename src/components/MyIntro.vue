<template>
  <div id="siteintro">
    <div class="golden_words">AWARD WINNING</div>
    <h2 class="decorated_text">Pro Barbers</h2>
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
#siteintro {
  background-image: url('../assets/img/avadabarbers-about-introbackground.jpg');
  clip-path: polygon(100% 0, 100% 100%, 50% 80%, 0% 100%, 0% 0%);
  object-fit: cover;
  background-position: top;
  background-repeat: no-repeat;
  text-align: center;
  padding-top: 100px;
  padding-bottom: 150px;

  h2 {
    padding-top: 10px;
    padding-bottom: 40px;
  }
}
</style>
