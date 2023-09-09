<template>
  <button class="btn">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: "my-button",
};
</script>

<style scoped>
.btn {
  padding: 10px 15px;
  background: none;
  color: teal;
  border: 1px solid teal;
  border-bottom-left-radius: 12px;
  border-top-right-radius: 12px;
}
.btn:hover {
  background: teal;
  color: #ffff;
}
</style>
