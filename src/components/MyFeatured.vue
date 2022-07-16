<template>
  <div id="sitefeatured">
    <div class="container">
      <div class="entire_featured">
        <div class="featured_box">
          <div class="col_sx">
            <img
              src="../assets/img/shaving_butter-200x200.png"
              alt="immagine crema da barba"
            />
          </div>
          <div class="col_dx">
            <div class="golden_words">THIS MONTH'S FEATURED PRODUT</div>
            <h2>Shaving Butter</h2>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus
              nisi maiores exercitationem alias adipisci obcaecati magnam eius
              quae sit! Quos odio quibusdam magnam delectus amet.
            </p>
            <button class="golden_btn">BUY NOW</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MyFeatured',
};
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
@import '../assets/style/common.scss';
.entire_featured {
  position: relative;
  width: 100%;
  height: 500px;
  .featured_box {
    width: 100%;
    border-top: 5px solid $main_color;
    display: flex;
    justify-content: space-between;
    position: absolute;
    left: 0%;
    top: -15%;
    .col_sx {
      width: 40%;
      background-image: url('../assets/img/avadabarbers-cta-background.jpg');
      object-fit: contain;
    }
    .col_dx {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: flex-start;
      width: 60%;
      padding: 40px;
      background-color: #121413;
      div {
        font-size: 1rem;
      }
      h2 {
        color: $secondary_color;
        font-size: 4rem;
        padding-top: 10px;
        padding-bottom: 30px;
      }
      p {
        color: $secondary_color;
        margin-bottom: 30px;
      }
    }
  }
}
</style>
