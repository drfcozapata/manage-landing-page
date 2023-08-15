<script setup>
	import HeaderComponent from './components/HeaderComponent.vue';
	import MainComponent from './components/MainComponent.vue';
	import FooterComponent from './components/FooterComponent.vue';

	const screenWidth = window.screen.width;
	console.log(screenWidth);
</script>

<template>
	<HeaderComponent />
	<MainComponent />
	<FooterComponent />
</template>

<style scoped>
	/*  */
</style>
