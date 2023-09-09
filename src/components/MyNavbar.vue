<template>
  <heder class="navbar">
    <img
      class="logo"
      src="../imeges/lazarenko.png"
      width="60"
      alt="Ania Lazarenko"
      @click="$router.push('/')"
    />
    <div class="navbar__btns">
      <my-button class="navbar-btn" @click="$router.push('/post')">Пости</my-button>
      <my-button class="navbar-btn" @click="$router.push('/about')" style="margin-left: 20px"
        >Про мене</my-button
      >
      <my-button class="navbar-btn" @click="$router.push('/store')" style="margin-left: 20px"
        >store</my-button
      >
    </div>
  </heder>
</template>

<script>
export default {};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Caveat:wght@400;500;600;700&display=swap");
.navbar {
  padding: 30px;
  height: 50px;

  box-shadow: 2px 2px 4px rgb(77, 78, 75);
  display: flex;
  align-items: center;
}
.navbar__btns {
  margin-left: auto;
 
}
.navbar-btn{
   font-family: "Caveat", cursive;
    font-size: 18px;
}
.logo {
  cursor: pointer;
}
.logo:hover {
  transform: translate(2px, 5%);
}
</style>

<!-- background: linear-gradient(135deg,rgb(2, 87, 23), orange 60%, cyan); -->
