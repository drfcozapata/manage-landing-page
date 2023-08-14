<script setup>
	//
</script>

<template>
	<section class="flex justify-between items-center py-28">
		<article class="w-[40%] flex flex-col gap-10">
			<h1 class="text-[50px] font-semibold text-dark-blue leading-[62px]">
				Bring everyone together to build better products.
			</h1>
			<p class="text-dark-grayish-blue pr-32">
				Manage makes it simple for software teams to plan day-to-day tasks while keeping
				the larger team goals in view.
			</p>
			<button class="bg-bright-red shadow-br text-white rounded-[32px]">
				Get Started
			</button>
		</article>
		<article class="w-[60%] flex justify-end">
			<img src="illustration-intro.svg" alt="" />
		</article>
	</section>
</template>

<style lang="scss" scoped>
	@media (max-width: 1920px) {
		section {
			margin-bottom: 30px;
			article {
				h1 {
					font-size: 60px;
					line-height: 74px;
				}
				p {
					font-size: 19px;
					padding-right: 180px;
				}
				img {
					width: 80%;
				}
			}
		}
	}
	@media (max-width: 1440px) {
		section {
			margin-bottom: 10px;
			article {
				h1 {
					font-size: 52px;
					line-height: 66px;
				}
				p {
					font-size: 16px;
					padding-right: 120px;
				}
				img {
					width: 85%;
				}
			}
		}
	}
	@media (max-width: 1366px) {
		h1 {
			font-size: 48px;
			line-height: 60px;
		}
		p {
			font-size: 15px;
			padding-right: 90px;
		}
		img {
			width: 83%;
		}
	}
	@media (max-width: 1280px) {
		section {
			margin-bottom: 0px;
			article {
				h1 {
					font-size: 46px;
					line-height: 1.3;
				}
				p {
					font-size: 14px;
					padding-right: 150px;
				}
				img {
					width: 80%;
				}
			}
		}
	}
	@media (max-width: 420px) {
		section {
			flex-direction: column-reverse;
			margin-bottom: 0px;
			padding: 60px 0;
			article {
				gap: 10px;
				width: 100%;
				justify-content: center;
				text-align: center;
				h1 {
					font-size: 36px;
					line-height: 1.3;
				}
				p {
					font-size: 16px;
					padding: 0px;
					margin-bottom: 20px;
				}
				button {
					margin: 0 auto;
					padding: 11px 22px;
				}
				img {
					width: 100%;
				}
			}
		}
	}
</style>
