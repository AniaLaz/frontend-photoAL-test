<template>
  <div class="main">
    <my-hero/>
    <BoxContainer>
    <div class="about">
      <div>
        <h2>Про мене</h2>
        <p class="text">
          Мене звати Аня і я хочу стати вашим сімейним фотографом. Я не
          представляю себе без камери, я обожнюю ловити справжні щирі почуття та
          зберігати їх на світлині. Я отримую неймовірне задоволення від
          спілкування з дітками під час зйомки. Дітей фотографувати одночасно і
          найлегше, бо в них завжди справжні емоції але і найважче, бо зловити в
          якісному знимку маленьке шило не так і легко. Так діти, то моє
          захоплення. Але і дорослих я не залишу без уваги, не хвилюйтеся.
        </p>
      </div>
            <img src="../imeges/ania.jpg" alt="Аня Лазаренко" class="img" />
    </div>
        <div>
      <h2>Що я роблю</h2>
      <WhatIDo/>
    </div>
    </BoxContainer>

  </div>
</template>

<script>
import MyHero from "@/components/MyHero";
import WhatIDo from "@/components/WhatIDo.vue";
import BoxContainer from "@/components/shared/BoxContainer";
export default {
  name: "my-main",
  components: {
    BoxContainer,
    MyHero,
    WhatIDo
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Pacifico&display=swap");
h2 {
  color: teal;
}
.main {
  text-align: center;
}
.text {
  font-family: "Pacifico", cursive;
  text-align: left;
  margin-bottom: 20px;
  font-size: 20px;
  line-height: 20px;
  margin-right: 20px;
  padding-left: 30px;
}
.about {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 20px;
}
.img {
  max-width: 200px;
  max-height: 100%;
  box-shadow: 2px 2px 4px rgb(77, 78, 75);
}
</style>
