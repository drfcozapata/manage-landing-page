<script setup>
	//
</script>

<template>
	<VueFinalModal
		class="flex justify-center items-center relative"
		content-class="flex flex-col mx-auto -mt-[480px] py-10 px-28 bg-white rounded space-y-2"
	>
		<!-- <img
			src="/icon-close.svg"
			alt=""
			@click="emit('confirm')"
			class="-top-40 -right-40 w-6 h-6 cursor-pointer"
		/> -->
		<ul
			class="flex flex-col gap-6 justify-center items-center text-dark-blue menu text-[16px] cursor-pointer"
		>
			<li class="hover:text-dark-grayish-blue">Pricing</li>
			<li class="hover:text-dark-grayish-blue">Product</li>
			<li class="hover:text-dark-grayish-blue">About Us</li>
			<li class="hover:text-dark-grayish-blue">Careers</li>
			<li class="hover:text-dark-grayish-blue">Community</li>
		</ul>
	</VueFinalModal>
</template>

<style scoped>
	li {
		font-weight: 700;
	}
</style>
