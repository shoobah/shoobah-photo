<template>
    <div>
        <Logo color="#F75C03" />
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
    color: {
      type: String,
      default: "#000"
    }
  },
  computed: {
    colorStyle: function getColorStyle() {
      return {
        color: this.color
      };
    }
  }
};
</script>

<style scoped>
#logo-text {
  font-size: 2em;
  font-family: Frijole, sans-serif;
  padding-left: 20px;
  line-height: 3em;
}
</style>



