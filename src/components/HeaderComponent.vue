<script setup>
	import BigHero from './header/BigHero.vue';
	import NavBar from './header/NavBar.vue';

	//
</script>

<template>
	<header class="container mx-auto relative pt-6 px-16">
		<img src="/bg-tablet-pattern.svg" alt="" />
		<NavBar />
		<BigHero />
	</header>
</template>

<style lang="scss" scoped>
	img {
		position: absolute;
		height: 105%;
		top: -256px;
		right: -325px;
		z-index: -10;
	}
	@media (max-width: 1920px) {
		header {
			padding-top: 60px;
			img {
				height: 105%;
				top: -270px;
				right: -340px;
			}
		}
	}
	@media (max-width: 1440px) {
		header {
			padding-top: 50px;
			img {
				height: 98%;
				top: -180px;
				right: -260px;
			}
		}
	}
	@media (max-width: 1366px) {
		img {
			height: 96%;
			top: -160px;
			right: -240px;
		}
	}
	@media (max-width: 1280px) {
		header {
			padding-top: 40px;
			img {
				height: 95%;
				top: -150px;
				right: -225px;
			}
		}
	}
	@media (max-width: 375px) {
		header {
			padding: 15px 25px 40px 25px;
			margin: 0;
			img {
				max-width: 450px;
				height: auto;
				top: -105px;
				right: -130px;
			}
		}
	}
</style>
