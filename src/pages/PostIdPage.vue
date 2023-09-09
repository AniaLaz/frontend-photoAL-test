<template>
  <div class="onePost">
    <h1>{{ this.post.title }}</h1>
    <div v-if="this.post.url">
      <img :src="this.post.url" :alt="this.post.title" class="imgPhoto" />
    </div>
    <div v-else>...іде завантаження</div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      post: {},
    //   isPostsLoading: false,
    };
  },
  methods: {
    async fetchPostById() {
      console.log("fetch");
      const myId = this.$route.params.id;
      console.log("id", myId);
    //   this.isPostsLoading = true;
      try {
        const response = await axios.get(
          ` https://backend-photoal-98ep.onrender.com/api/photos/${myId} `
        );
        this.post = response.data;
        console.log(response);
      } catch (error) {
        alert(error.message);
        console.log("err", error.message);
      } finally {
        // this.isPostsLoading = false;
      }
    },
  },
  mounted() {
    this.fetchPostById();
  },
};
</script>

<style scoped>
.onePost {
  text-align: center;
  width: 100%;
}
.imgPhoto {
  max-height: 80vh;
  max-width: 100vw;
  margin-right: 20px;
}
</style>
