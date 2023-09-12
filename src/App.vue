<template>
  <div class="app">
    <BoxContainer>
      <MyNavbar />
    </BoxContainer>
    <div>
      <router-view />
    </div>
    <BoxContainer>
      <MyFooter />
    </BoxContainer>
  </div>
</template>

<script>
import MyNavbar from "@/components/MyNavbar";
import MyFooter from "./components/MyFooter.vue";
import BoxContainer from "@/components/shared/BoxContainer";
export default {
  components: {
    BoxContainer,
    MyNavbar,
    MyFooter,
  },
};
</script>

<style scoped>
* {
  margin: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-bottom: 60px;
}
</style>

<!-- npm run serve -->

<!-- DEPLOY -->

<!-- git add .   --------- зберігаєм зміни на git-->
<!-- git commit -m "what i do"     ----------- робимо коміт-->
<!-- git push -->
<!-- npm run deploy    ------------- робимо деплой проекту-->
