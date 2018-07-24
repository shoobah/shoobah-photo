<template>
	<div id="app">
		<Header text="Sjöbergs fotolabb" color="#FFFFFA"/>
		<div id="main">
			<image-grid />
		</div>
	</div>
</template>

<script>
import Header from "./components/Header.vue";
import ImageGrid from "./components/ImageGrid.vue";

export default {
	name: "app",
	components: {
		Header,
		ImageGrid
	}
};
</script>

<style src="./style/main.css">
</style>
