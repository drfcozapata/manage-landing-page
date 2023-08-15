<script setup>
	import DiferentAbout from './main/DiferentAbout.vue';
	import TestimonialsSlider from './main/TestimonialsSlider.vue';

	//
</script>

<template>
	<main class="mx-auto relative">
		<img src="/bg-tablet-pattern.svg" alt="" />
		<DiferentAbout />
		<TestimonialsSlider />
	</main>
</template>

<style lang="scss" scoped>
	img {
		position: absolute;
		height: 75%;
		top: 260px;
		left: -700px;
		z-index: -10;
	}
	@media (max-width: 1920px) {
		img {
			height: 77%;
			top: 290px;
			left: -680px;
		}
	}
	@media (max-width: 1440px) {
		img {
			height: 75%;
			top: 250px;
			left: -580px;
		}
	}
	@media (max-width: 1366px) {
		img {
			height: 75%;
			top: 240px;
			left: -550px;
		}
	}
	@media (max-width: 1280px) {
		img {
			height: 70%;
			top: 230px;
			left: -470px;
		}
	}
	@media (max-width: 420px) {
		main {
			padding: 0;
		}
		img {
			width: 90%;
			height: auto;
			top: -340px;
			left: 240px;
		}
	}
</style>
