<template>
  <div id="sitereviews">
    <div class="golden_words">WHAT PEOPLE SAY</div>
    <h2 class="decorated_text">Reviews</h2>

    <div class="container">
      <div class="col_box">
        <div class="col_sx">
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Molestias,
            ipsam voluptates ad dolorum quaerat doloremque eius ducimus illum
            eveniet? Iusto dolorum voluptatem nulla nihil quo, consectetur quae
            ea enim doloremque?
          </p>
          <img
            src="../assets/img/avadabarbers-trimcut-gallery6-400x400.jpg"
            alt="Immagine di John Doe che guarda a sinistra"
          />
          <div class="who_said"><i class="golden_words">John Doe</i></div>
        </div>
        <div class="col_mid">
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Molestias,
            ipsam voluptates ad dolorum quaerat doloremque eius ducimus illum
            eveniet? Iusto dolorum voluptatem nulla nihil quo, consectetur quae
            ea enim doloremque?
          </p>
          <img
            src="../assets/img/avadabarbers-trimcut-gallery7-400x402.jpg"
            alt="Immagine di Pete Jones che guarda dritto in camera"
          />
          <div class="who_said"><i class="golden_words">Pete Jones</i></div>
        </div>
        <div class="col_dx">
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Molestias,
            ipsam voluptates ad dolorum quaerat doloremque eius ducimus illum
            eveniet? Iusto dolorum voluptatem nulla nihil quo, consectetur quae
            ea enim doloremque?
          </p>
          <img
            src="../assets/img/avadabarbers-trimcut-gallery3-400x402.jpg"
            alt="Immagine di Mark Wilson che guarda leggermente a sinistra"
          />
          <div class="who_said"><i class="golden_words">Mark Wilson</i></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MyReviews',
};
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
@import '../assets/style/common.scss';
#sitereviews {
  text-align: center;
  padding-top: 100px;
  padding-bottom: 50px;
  h2 {
    color: $secondary_color;
    font-size: 4rem;
    padding-top: 10px;
    padding-bottom: 40px;
  }
}
.col_box {
  display: flex;
  .col_sx,
  .col_mid,
  .col_dx {
    padding-inline: 70px;
  }
  p {
    margin-bottom: 20px;
  }
  img {
    width: 50%;
    margin: 0 auto;
    border-radius: 50%;
  }
  .golden_words {
    padding-top: 20px;
  }
}
.who_said {
  padding-top: 20px;
}
</style>
