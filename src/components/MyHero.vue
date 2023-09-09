<template>
  <section class="hero">
    <div class="container">
      <h1 class="hero-title">Кольори життя</h1>
      <my-button type="button" class="hero-button">
        Замовити послугу
      </my-button>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style scoped>
.hero {
  
  background-color: yellow;
  padding-top: 118px;
  padding-bottom: 118px;

  height: 130px;
  max-width: 1600px;
  margin-left: auto;
  margin-right: auto;
  margin-top: 5px;
  background-image: linear-gradient(
      to right,
      rgba(0,128,0, 0.3),
      rgba(104, 26, 248, 0.4)
    ),
    url("../imeges/hero2.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.hero-title {
  margin-bottom: 30px;

  margin-left: auto;
  margin-right: auto;

  font-family: "Press+Start+2P", san-serif;
  font-weight: 900;
  font-size: 40px;
  line-height: 1.62;
  text-align: center;
  letter-spacing: 0.06em;
  text-transform: uppercase;
  color: white;
  text-shadow: 3px 3px 5px rgba(13, 184, 13);
}
.hero-button {
  background-color: rgba(250, 157, 80);
}
</style>
