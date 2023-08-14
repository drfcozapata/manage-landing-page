<script setup>
	const props = defineProps({
		show: Boolean,
	});
</script>

<template>
	<Transition name="modal">
		<div v-if="show" class="modal-mask">
			<img
				src="/icon-close.svg"
				alt=""
				height="20"
				class="absolute top-[38px] right-[28px] cursor-pointer"
				@click="$emit('close')"
			/>
			<div class="modal-container">
				<div class="modal-body">
					<ul
						class="flex flex-col gap-6 justify-center mx-auto items-center rounded bg-white text-dark-blue menu text-[16px]"
					>
						<li class="hover:text-dark-grayish-blue cursor-pointer">Pricing</li>
						<li class="hover:text-dark-grayish-blue cursor-pointer">Product</li>
						<li class="hover:text-dark-grayish-blue cursor-pointer">About Us</li>
						<li class="hover:text-dark-grayish-blue cursor-pointer">Careers</li>
						<li class="hover:text-dark-grayish-blue cursor-pointer">Community</li>
					</ul>
				</div>
			</div>
		</div>
	</Transition>
</template>

<style scoped>
	.modal-mask {
		position: fixed;
		z-index: 9998;
		top: 0;
		left: 0;
		width: 375px;
		height: 100%;
		background: linear-gradient(
			0deg,
			hsl(228, 39%, 23%, 0.9) 0%,
			hsl(228, 39%, 23%, 0.6) 62%,
			rgba(255, 255, 255, 0) 100%
		);
		display: flex;
		padding-left: 30px;
		transition: opacity 0.3s ease;
	}

	.modal-container {
		position: absolute;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding: 40px 112px;
		border-radius: 3px;
		margin-top: 100px;
		max-width: 325px;
		background-color: #fff;
		box-shadow: 0 2px 8px rgba(0, 0, 0, 0.33);
		transition: all 0.3s ease;
	}
	.modal-body {
		margin: 0;
	}
	li {
		font-weight: 700;
	}
</style>
