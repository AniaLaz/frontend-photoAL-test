<template>
  <div class="post">
    <div class="postContent">
      <img
        :src="imgSrc"
        :alt="title"
        class="imgPhoto"
        @click="$emit('show', post)"
      />
      <div>
        <div><strong>Назва:</strong>{{ title }}</div>
        <div><strong>Опис:</strong>{{ post.body }}</div>
        <div class="post__btns">
          <my-button class="btnOupen" @click="$router.push(`/post/${post._id}`)"
            >відкрити
          </my-button>
          <!-- <my-button class="btnDalite" @click="$emit('remove', post)"
            >Стерти
          </my-button> -->
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    post: {
      tipe: Object,
      required: true,
    },
    title: {
      tipe: String,
      default: "",
    },
    imgSrc: {
      tipe: String,
      default:
        "https://img3.akspic.ru/previews/5/5/4/1/7/171455/171455-zhivopis-illustracia-art-voda-oblako-550x310.jpg",
    },
  },
  methods: {},
};
</script>

<style scoped>
.post {
  padding: 15px;
  border: 2px solid teal;
  text-align: left;
  max-width: 45%;
  gap: 20px;
}
.post__btns{
  display: flex;
}
.btnDalite {
  margin-top: 120px;
  margin-left: 15px;
}
.btnOupen {
  margin-top: 120px;
  margin-left: auto;

}
.imgPhoto {
  width: 300px;
  height: 300px;
  margin-right: 20px;
}
.postContent {
  display: flex;
}
</style>
