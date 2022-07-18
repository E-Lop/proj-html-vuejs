<template>
  <div id="siteblog">
    <div class="entire_blogpost">
      <div class="golden_words">TALES FROM THE BARBER SHOP</div>
      <h2 class="decorated_text">Recent Blog Posts</h2>
      <div class="container">
        <div class="col_box">
          <div class="col_sx">
            <img
              src="../assets/img/avadabarbers-second-blog-700x441.jpg"
              alt="Immagine per blogpost sull'apertura del barber shop con un pennello da barba e la luce cilindrica a fasce alternate bianche rosse e blue tipica dei barbieri"
            />
            <div class="golden_words fatface_gold">Avada Barbers Now Open</div>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat
              eos debitis tenetur dolorem veniam!
            </p>
          </div>
          <div class="col_mid">
            <img
              src="../assets/img/avadabarbers-choosing-blog-700x441.jpg"
              alt="Immagine per blogpost su come scegliere il barbiere giusto con la foto dell'interno di un salone da barba e in primo piano due sedie ma barbiere vuote"
            />
            <div class="golden_words fatface_gold">
              Choosing The Right Barber
            </div>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat
              eos debitis tenetur dolorem veniam!
            </p>
          </div>
          <div class="col_dx">
            <img
              src="../assets/img/avadabarbers-ourservice-blog-700x441.jpg"
              alt="Immagine per blogpost sulla guida ai servizi offerti dalla catena di barbieri Avada con il primo piano di un barbiere che cura la barba di un cliente seduto su una sedia da barbiere e coperto da un telo che impedisce a peli di barba e capelli di finire sui sui vestiti"
            />
            <div class="golden_words fatface_gold">Quick Service Guide</div>
            <p>
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat
              eos debitis tenetur dolorem veniam!
            </p>
          </div>
        </div>
      </div>
      <button class="golden_btn">READ MORE FROM OUR BLOG</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MyBlogPost',
};
</script>

<style lang="scss" scoped>
.entire_blogpost {
  background-color: #f5f5f5;
  clip-path: polygon(100% 0%, 100% 100%, 0 100%, 0 0, 50% 10%);
  text-align: center;
  padding-top: 200px;
  padding-bottom: 70px;
  .golden_words {
    padding-bottom: 10px;
  }
}
.col_box {
  display: flex;
  justify-content: space-between;
  margin-top: 50px;
  margin-bottom: 50px;
}
.col_sx {
  width: 32%;
  padding-inline: 10px;
  div {
    padding-block: 20px;
  }
  img {
    margin: 0 auto;
  }
}
.col_mid {
  width: 32%;
  padding-inline: 10px;
  div {
    padding-block: 20px;
  }
  img {
    margin: 0 auto;
  }
  p {
    padding-inline: 20px;
  }
}
.col_dx {
  width: 32%;
  padding-inline: 10px;
  div {
    padding-block: 20px;
  }
  img {
    margin: 0 auto;
  }
}
</style>
