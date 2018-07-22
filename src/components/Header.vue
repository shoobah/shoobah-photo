<template>
    <div>
        <Logo :color="baseColor" />
        <span id="logo-text" :style="colorStyle">{{text}}</span>
    </div>
</template>

<script>
import Logo from "./Logo.vue";

export default {
  name: "Header",
  components: {
    Logo
  },
  props: {
    text: {
      type: String,
      default: "---"
    },
    baseColor: {
      type: String,
      default: "#000"
    }
  },
  computed: {
    colorStyle: function getColorStyle() {
      return {
        color: this.baseColor
      };
    }
  }
};
</script>

<style scoped>
#logo-text {
  font-size: 2em;
  font-family: Gloria Hallelujah, sans-serif;
  padding-left: 20px;
  line-height: 3em;
}
</style>



