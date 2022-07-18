<template>
  <div id="siteshop">
    <div class="entire_siteshop">
      <h4 class="golden_words">WE HAVE YOU COVERED</h4>
      <h2 class="decorated_text">Avada Grooming Products</h2>
      <div class="products_box">
        <div class="col1">
          <img
            src="../assets/img/brush_dark-400x400.png"
            alt="immagine pennello da barba"
          />
          <h3 class="golden_words fatface_gold">Brush</h3>
          <div class="price golden_words">$15.00</div>
        </div>
        <div class="col2">
          <img
            src="../assets/img/scissors-400x400.png"
            alt="immagine forbici da baribiere"
          />
          <h3 class="golden_words fatface_gold">Scissors</h3>
          <div class="price golden_words">$85.00</div>
        </div>
        <div class="col3">
          <img
            src="../assets/img/hot_oil_dark-400x400.png"
            alt="immagine lozione da barba"
          />
          <h3 class="golden_words fatface_gold">Hot Oil</h3>
          <div class="price golden_words">$15.00</div>
        </div>
        <div class="col4">
          <img
            src="../assets/img/straight_razor_dark-400x400.png"
            alt="immagine rasoio da barbiere"
          />
          <h3 class="golden_words fatface_gold">Straight Razor</h3>
          <div class="price golden_words">$30.00</div>
        </div>
      </div>
      <button class="golden_btn">SHOP OUR PRODUCT RANGE</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MyShop',
};
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
@import '../assets/style/common.scss';
.entire_siteshop {
  background-image: url('../assets/img/avadabarbers-reviewsbackground.jpg');
  object-fit: fill;
  background-position: top;
  background-repeat: no-repeat;
  text-align: center;
  padding-top: 100px;
  padding-bottom: 150px;
  h2 {
    padding-top: 30px;
    padding-bottom: 80px;
  }
}
.products_box {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  .price {
    padding-top: 10px;
    font-size: 1rem;
  }
}
button {
  margin-top: 50px;
}
</style>
