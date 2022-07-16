<template>
  <div id="siteservices">
    <div class="golden_words">MENS GROOMING</div>
    <h2>Services</h2>

    <div class="container">
      <div class="col_box">
        <div class="col_sx">
          <img
            src="../assets/img/avadabarbers-trimcut-icon-before.png"
            alt="Immagine macchinetta per capelli per il servizio Trim&Cut"
          />
          <div class="golden_words">Trim & Cut</div>
          <p>
            Avada Barbers are experts in the lickety split trim and hair cut.
            Quick but careful and ridiculously good looking.
          </p>
        </div>
        <div class="col_mid">
          <img
            src="../assets/img/avadabarbers-washndry-icon.png"
            alt="Immagine bottiglietta con sapone"
          />
          <div class="golden_words">Wash & Dry</div>
          <p>
            Take a seat in our fine leather chairs, lean back and let us lather
            you a fresh head in a luxurious fashion.
          </p>
        </div>
        <div class="col_dx">
          <img
            src="../assets/img/avadabarbers-beardtrim-icon.png"
            alt="Immagine macchinetta per capelli per il servizio Trim&Cut"
          />
          <div class="golden_words">Beard Tidy</div>
          <p>
            Tame the tangles and untidy facial hair like a gentleman with our
            Beard Tidy services from Avada Barbers.
          </p>
        </div>
      </div>
      <button class="golden_btn">READ ABOUT OUR SERVICES</button>
    </div>
    <div class="triangle"></div>
  </div>
</template>

<script>
export default {
  name: 'MyServices',
};
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
@import '../assets/style/common.scss';
#siteservices {
  text-align: center;
  padding-top: 100px;
  h2 {
    color: $secondary_color;
    font-size: 4rem;
    padding-top: 10px;
    padding-bottom: 40px;
  }
  .triangle {
    clip-path: polygon(50% 50%, 0% 100%, 100% 100%);
    background-color: #121314;
    height: 150px;
    background-color: #121314;
  }
  .col_box {
    display: flex;
    margin-bottom: 50px;
  }
  .col_sx {
    width: 30%;
    padding-inline: 20px;
    div {
      padding-block: 20px;
    }
    img {
      width: 50px;
      margin: 0 auto;
    }
  }
  .col_mid {
    width: 40%;
    padding-inline: 20px;
    div {
      padding-block: 20px;
    }
    img {
      width: 65px;
      margin: 0 auto;
    }
    p {
      padding-inline: 20px;
    }
  }
  .col_dx {
    width: 30%;
    padding-inline: 20px;
    div {
      padding-block: 20px;
    }
    img {
      width: 50px;
      margin: 0 auto;
    }
  }
}
</style>
