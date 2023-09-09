<template>
  <div>
    <ul class="we-doing-list list">
      <li class="we-doing-item">
        <img class="we-doing-img" src="../imeges/children.jpg" alt="дитина" width="371" />
        <p class="we-doing-img-title">Дитяча фотографія</p>
      </li>
      <li class="we-doing-item">
        <img class="we-doing-img" src="../imeges/femily.jpg" alt="сім'я" width="371" />
        <p class="we-doing-img-title">Сімейна зйомка</p>
      </li>
      <li class="we-doing-item">
        <img class="we-doing-img" src="../imeges/love-story.jpg" alt="закохані" width="371" />
        <p class="we-doing-img-title" lang="en">love story</p>
      </li>
      <li class="we-doing-item">
        <img class="we-doing-img" src="../imeges/clas.jpg" alt="однокласники" width="371" />
        <p class="we-doing-img-title">шкільна фотосесія</p>
      </li>
      <li class="we-doing-item">
        <img
        class="we-doing-img"
          src="../imeges/christening.jpg"
          alt="хрещення дитини"
          width="371"
        />
        <p class="we-doing-img-title">Хрестини</p>
      </li>
      <li class="we-doing-item">
        <img class="we-doing-img" src="../imeges/albom.jpg" alt="фото-альбоми" width="371" />
        <p class="we-doing-img-title">фото-альбоми</p>
      </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
ul {
  padding-inline-start: 0;
  margin-block-start: 0;
  margin-block-end: 0;
}

.list {
  list-style: none;
}
.we-doing-list {
  display: flex;
  margin-top: 50px;
  gap: 30px;
  flex-wrap: wrap;
}
.we-doing-img{
      width: 100%;

}

.we-doing-item {
  position: relative;
  width: calc((100% - 60px) / 3);
}

.we-doing-item:hover {
  transform: translate(2px, 5%);
}

.we-doing-img-title {
  position: absolute;
  bottom: 0;
  display: flex;
  font-family: "Caveat";
  font-style: normal;
  text-align: center;
  letter-spacing: 0.03em;
  text-transform: uppercase;
  align-items: center;
  justify-content: center;
  width: 100%;
  border: 0;
  color: white;
  background: rgba(47, 48, 58, 0.8);

  font-weight: 700;
  font-size: 14px;
  height: 70px;
}
</style>
