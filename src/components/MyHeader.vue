<template>
  <div class="entire_header">
    <div class="container">
      <div class="navbar">
        <div class="navbar_left">
          <a class="navbar-brand" href="#">
            <img
              src="../assets/img/avadabarbers-logo-x1.png"
              alt="Logo Avada Barbers"
            />
          </a>
        </div>
        <div class="navbar_icons">
          <!-- icona shopping cart -->
          <a href="#"><i class="fa-solid fa-cart-shopping"></i></a>
          <!-- Collapse button -->
          <button class="navbar-toggler" type="button">
            <span class="burer"><i class="fa-solid fa-bars"></i></span>
          </button>
        </div>
      </div>
      <!-- contenuto al centro dell'header -->
      <div class="header_hero_content">
        <div class="header_hero_left">
          <h1>Barber Shop</h1>
          <div class="golden_bar"></div>
          <div class="claim">The Pinnacle of Male Grooming</div>
          <button class="learn_btn">LEARN MORE</button>
        </div>
        <div class="header_hero_right">
          <img
            src="../assets/img/avadabarbers_hero_focalmirror-600x825.png"
            alt="immagine barbiere al lavoro"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MyHeader',
};
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
.entire_header {
  background-image: url('../assets/img/avadabarbers-homepage-hero-bg.jpg');
  object-fit: cover;
  background-position: top;
  background-repeat: no-repeat;
}
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 20px;
  i {
    color: white;
    font-size: 1.5rem;
  }
}
.navbar-brand {
  img {
    width: 170px;
  }
}
.header_hero_content {
  width: 100%;
  display: flex;
}
.header_hero_left {
  width: 50%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  color: white;
  h1 {
    font-size: 3rem;
  }
  .golden_bar {
    height: 2px;
    width: 200px;
    background-color: $main_color;
    margin-block: 30px;
  }
  .claim {
    margin-bottom: 30px;
    font-size: 1.2rem;
    color: $secondary_color;
  }
  .learn_btn {
    color: $main_color;
    border: 1px solid $main_color;
    padding: 15px 30px;
    background-color: transparent;
  }
}
.header_hero_right {
  width: 50%;
}
</style>
