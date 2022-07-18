<template>
  <section id="sitefooter">
    <!-- PARTE SUPERIORE DEL FOOTER -->
    <div class="footer_top">
      <div class="container">
        <div class="footertop_box">
          <!-- parte superiore, colonna sinistra -->
          <div class="footertop_left_col">
            <img
              src="../assets/img/avadabarbers_footer_shop_image-600x468.png"
              alt="Immagine esempio prodotti in vendita"
            />
            <div class="golden_btn">SHOP OUR RANGE NOW</div>
          </div>
          <!-- parte superiore, colonna centrale -->
          <div class="footertop_mid_col">
            <img
              src="../assets/img/avadabarbers-logo-x1.png"
              alt="Logo Avada Barbers"
            />
            <div class="brickMortar">
              <ul>
                <!-- informazioni generate dinamicamente da props -->
                <li v-for="(element, index) in shopInfo" :key="index">
                  {{ element }}
                </li>
              </ul>
              <div class="follow">FOLLOW US</div>
              <div class="social">
                <ul>
                  <li>
                    <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                  </li>
                  <li>
                    <a href="#"><i class="fa-brands fa-twitter"></i></a>
                  </li>
                  <li>
                    <a href="#"><i class="fa-brands fa-youtube"></i></a>
                  </li>
                  <li>
                    <a href="#"><i class="fa-brands fa-instagram"></i></a>
                  </li>
                </ul>
              </div>
            </div>
          </div>
          <!-- parte superiore, colonna destra -->
          <div class="footertop_right_col">
            <img
              src="../assets/img/avadabarbers_footer_appointment_image-600x468.png"
              alt="Immagine taglio di capelli per riservare una prenotazione"
            />

            <div class="golden_btn">BOOK YOUR APPOINTMENT</div>
          </div>
        </div>
      </div>
    </div>
    <!-- PARTE INFERIORE DEL FOOTER -->
    <div class="footer_bottom">
      <div class="copy_bottom">
        &#169; Copyright 2012-2020 | Avada Theme by ThemeFusion | All Rights
        Reserved | Powered by WordPress
      </div>
      <!-- link per tornare in cima alla pagina -->
      <div class="back_to_top">
        <a href="#header"><i class="fa-solid fa-chevron-up"></i></a>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'MyFooter',
  props: {
    shopInfo: Array,
  },
};
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
.footer_top {
  background-color: #121314;
}
.footertop_box {
  width: 100%;
  display: flex;
  padding-block: 50px;
}
.footertop_left_col {
  width: 30%;
}
.footertop_mid_col {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 40%;
  text-align: center;
  ul {
    padding-top: 30px;
    li {
      padding-block: 3px;
      color: $secondary_color;
    }
  }
  .follow {
    padding-top: 10px;
    color: $main_color;
    font-weight: bold;
  }
  .social {
    ul {
      display: flex;
      flex-direction: row;
      justify-content: center;
      li {
        padding-inline: 8px;
        font-size: 1.2rem;
      }
    }
  }
  img {
    width: 170px;
    margin: 0 auto;
  }
}
.footertop_right_col {
  width: 30%;
}
.footer_bottom {
  position: relative;
  .back_to_top {
    color: white;
    padding: 10px;
    background-color: #303030;
    position: fixed;
    bottom: 0;
    right: 5%;
  }
}
.copy_bottom {
  text-align: center;
  color: $secondary_color;
  padding-block: 50px;
  background-color: #161718;
}
</style>
