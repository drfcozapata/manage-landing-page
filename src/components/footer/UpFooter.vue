<template>
	<section class="bg-bright-red">
		<div class="container px-16 mx-auto flex justify-between relative up-footer">
			<img src="/bg-simplify-section-desktop.svg" alt="" class="img-desktop" />
			<img src="/bg-simplify-section-mobile.svg" alt="" class="img-mobile hidden" />
			<div class="container relative flex justify-between items-center py-14">
				<h2 class="text-4xl text-white font-semibold h2-desktop">
					Simplify how your team <br />works today.
				</h2>
				<h2 class="text-4xl text-white font-semibold h2-mobile hidden">
					Simplify how <br />your team works <br />today.
				</h2>
				<button class="text-bright-red shadow-br bg-white rounded-[32px]">
					Get Started
				</button>
			</div>
		</div>
	</section>
</template>

<style lang="scss" scoped>
	.up-footer img {
		position: absolute;
		top: -164px;
		right: -220px;
	}
	button:hover {
		background-color: hsl(13, 100%, 96%);
	}
	@media (max-width: 1920px) {
		.up-footer {
			img {
				width: 160%;
				height: auto;
			}
			div {
				padding: 70px 0;
			}
		}
	}
	@media (max-width: 1440px) {
		.up-footer {
			img {
				width: 120%;
				top: -100px;
			}
			div {
				padding: 70px 0;
			}
		}
	}
	@media (max-width: 1366px) {
		.up-footer {
			img {
				width: 110%;
				top: -120px;
			}
			div {
				padding: 60px 0;
			}
		}
	}
	@media (max-width: 1280px) {
		.up-footer {
			img {
				width: 95%;
				top: -110px;
			}
			div {
				padding: 55px 0;
			}
		}
	}
	@media (max-width: 420px) {
		.up-footer {
			padding: 0 20px;
			div {
				flex-direction: column;
				padding: 90px 0;
				gap: 25px;
				h2 {
					text-align: center;
					font-size: 34px;
					line-height: 44px;
				}
				.h2-desktop {
					display: none;
				}
				.h2-mobile {
					display: block;
				}
				button {
					height: 42px;
					font-weight: 700;
				}
			}
			.img-desktop {
				display: none;
			}
			.img-mobile {
				display: block;
			}
			img {
				height: 75%;
				width: 25%;
				top: 50px;
				left: 0;
			}
		}
	}
</style>
