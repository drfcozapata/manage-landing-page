<script setup>
	import { ref } from 'vue';
	import MenuModal from './MenuModal.vue';

	const showModal = ref(false);
</script>

<template>
	<nav class="pt-6 flex justify-between items-center relative">
		<img src="/logo.svg" alt="" class="logo" />
		<ul class="flex gap-8 justify-center text-very-dark-blue menu">
			<li>Pricing</li>
			<li>Product</li>
			<li>About Us</li>
			<li>Careers</li>
			<li>Community</li>
		</ul>
		<button class="bg-bright-red shadow-br text-white rounded-[32px] mr-7 btn-nav">
			Get Started
		</button>
		<img
			src="/icon-hamburger.svg"
			alt=""
			class="hidden hamburger"
			v-if="!showModal"
			@click="showModal = true"
		/>

		<!-- Modal Menu -->
		<Teleport to="body">
			<MenuModal :show="showModal" @close="showModal = false" />
		</Teleport>
	</nav>
</template>

<style lang="scss" scoped>
	li {
		color: hsl(228 39% 23%);
		font-weight: 500;
		cursor: pointer;

		&:hover {
			color: hsl(227, 12%, 61%);
		}
	}
	@media (max-width: 1920px) {
		img {
			width: 180px;
		}
	}
	@media (max-width: 1440px) {
		img {
			width: 156px;
		}
	}
	@media (max-width: 1366px) {
		img {
			width: 150px;
		}
	}
	@media (max-width: 1280px) {
		img {
			width: 144px;
		}
	}
	@media (max-width: 375px) {
		nav {
			.menu,
			.btn-nav {
				display: none;
			}
			.logo {
				width: 110px;
			}
			.hamburger {
				display: block;
				height: 20px;
				width: auto;
				cursor: pointer;
			}
		}
		img {
			width: 144px;
		}
	}
</style>
