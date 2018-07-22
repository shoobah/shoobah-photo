<template>
    <img :src="src" alt="">
</template>

<script>
export default {
  props: {
    src: {
      type: String,
      default: "No image"
    },
    title: {
      type: String,
      default: "Untitled"
    }
  }
};
</script>

<style scoped>
img {
  width: 300px;
}
</style>
