<template>
	<div id="grid">
		<small-image v-for="(image, index) in images" :key="index" :src="image.url" :style="imageStyle(index)" />
	</div>
</template>

<script>
import SmallImage from "./SmallImage.vue";

export default {
	name: "ImageGrid",
	data: function getData() {
		return {
			images: [
				{ url: "/images/_DSC0509.jpg" },
				{ url: "/images/_DSC0509.jpg" },
				{ url: "/images/_DSC0509.jpg" }
			]
		};
	},
	components: {
		SmallImage
	},
	computed: {
		imageStyle: function getImageStyle(index) {
			return {
				gridColumn: index
			};
		}
	}
};
</script>

<style scoped>
#grid {
	display: grid;
	grid-template-columns: 20% 20% 20% 20% 20%;
	grid-template-rows: 20% 20% 20% 20% 20%;
}
</style>
