<template>
	<div id="app">
		<Header text="Sjöbergs fotolabb" base-color="#FF0000"/>
	</div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Header from "./components/Header.vue";

export default {
  name: "app",
  components: {
    Header
  }
};
</script>

<style src="./style/main.css">
</style>
