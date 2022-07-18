<template>
  <section id="header">
    <div class="entire_header">
      <div class="container">
        <!-- navbar in cima all'header -->
        <div class="navbar">
          <div class="navbar_left">
            <!-- logo della compagnia -->
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
            <!-- burger menu -->
            <button
              @click="showBurgerMenu"
              class="navbar-toggler"
              type="button"
            >
              <span class="burger">
                <img
                  src="../assets/img/hamburger-button.png"
                  alt="Tasto burger menu"
                />
              </span>
            </button>
            <transition name="fade">
              <div v-if="dropdown_m" class="collapsed_menu">
                <ul>
                  <!-- lista dinamica di collegamenti alle varie section del sito -->
                  <li v-for="(element, index) in internalMap" :key="index">
                    <a
                      @click="closeTheMenu"
                      class="selected"
                      :href="element.id"
                      >{{ element.name }}</a
                    >
                  </li>
                </ul>
              </div>
            </transition>
          </div>
        </div>
        <!-- contenuto al centro dell'header -->
        <div class="header_hero_content">
          <!-- parte a sinistra con testi e bottone -->
          <div class="header_hero_left">
            <h1 class="decorated_text">Barber Shop</h1>
            <div class="golden_bar"></div>
            <div class="claim">The Pinnacle of Male Grooming</div>
            <button class="golden_btn">LEARN MORE</button>
          </div>
          <!-- parte sulla destra con immagine allo specchio -->
          <div class="header_hero_right">
            <img
              src="../assets/img/avadabarbers_hero_focalmirror-600x825.png"
              alt="immagine barbiere al lavoro"
            />
          </div>
          <!-- quadtati sfondo bianco a destra -->
          <div class="white_buttons">
            <div class="demos white_btn">
              <i class="fa-brands fa-atlassian"></i>
              <div>Demos</div>
            </div>
            <div class="sale white_btn">
              <div class="bargain">
                <div class="discount"><sup>$</sup>39</div>
              </div>
              <div>On Sale</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'MyHeader',
  props: {
    internalMap: Array,
  },
  data() {
    return {
      dropdown_m: false,
    };
  },
  methods: {
    closeTheMenu() {
      this.dropdown_m = false;
    },
    showBurgerMenu() {
      this.dropdown_m = !this.dropdown_m;
    },
  },
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
  position: relative;
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
.navbar-toggler {
  margin-left: 20px;
}
.navbar_icons {
  display: flex;
  align-items: center;
}
.burger {
  img {
    width: 24px;
    background: transparent;
  }
}
.collapsed_menu {
  color: white;
  position: absolute;
  right: 0;
  top: 100%;
  text-align: right;
  font-size: 1.5rem;
  li {
    padding-block: 5px;
    .selected:hover {
      color: $main_color;
    }
  }
}
// gestione effetto fade opacità del menu al click
.fade-enter-active,
.fade-leave.active {
  transition: opacity 1s;
}
.fade-enter,
.fade.leave-to {
  opacity: 0;
}
// contenuto al centro dell'header
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
    font-size: 5rem;
  }
  .golden_bar {
    height: 5px;
    width: 200px;
    background-color: $main_color;
    margin-block: 30px;
  }
  .claim {
    margin-bottom: 30px;
    font-size: 1.5rem;
    color: $secondary_color;
  }
}
// colonna
.header_hero_right {
  width: 50%;
}

// tasti sfondo bianco sulla destra position fixed
.white_buttons {
  position: fixed;
  right: 10px;
  top: 80px;
  z-index: 10;
}
.white_btn {
  width: 80px;
  height: 80px;
  border-radius: 5px;
  background-color: white;
  border: 1px solid black;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
}
.demos {
  i {
    font-size: 2rem;
  }
}
.sale {
  margin-top: 5px;
}
.bargain {
  color: #65bc7b;
  font-size: 2rem;
  font-weight: bold;
}
</style>
