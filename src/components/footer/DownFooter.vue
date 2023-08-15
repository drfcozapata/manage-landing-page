<template>
	<section class="bg-very-dark-blue">
		<div
			class="container flex justify-between items-start px-16 mx-auto py-14 down-footer"
		>
			<article class="flex flex-col gap-[82px] items-start text-white redes">
				<p class="text-dark-grayish-blue text-[13px] hidden">
					Copyright 2023. All Rights Reserved
				</p>
				<img src="/logo-w.svg" alt="" />
				<div class="flex gap-3">
					<a href=""
						><font-awesome-icon :icon="['fab', 'square-facebook']" class="w-5 h-5 icon"
					/></a>
					<a href=""
						><font-awesome-icon :icon="['fab', 'youtube']" class="w-5 h-5 icon"
					/></a>
					<a href=""
						><font-awesome-icon :icon="['fab', 'twitter']" class="w-5 h-5 icon"
					/></a>
					<a href=""
						><font-awesome-icon :icon="['fab', 'pinterest']" class="w-5 h-5 icon"
					/></a>
					<a href=""
						><font-awesome-icon :icon="['fab', 'instagram']" class="w-5 h-5 icon"
					/></a>
				</div>
			</article>
			<div class="flex flex-links">
				<article class="flex flex-col gap-3 text-white links">
					<a href="">Home</a>
					<a href="">Pricing</a>
					<a href="">Products</a>
					<a href="">About Us</a>
				</article>
				<article class="flex flex-col justify-start gap-3 text-white links">
					<a href="">Careers</a>
					<a href="">Community</a>
					<a href="">Privacy Policy</a>
				</article>
			</div>
			<article class="flex flex-col gap-[72px] justify-between items-end copy">
				<div class="flex gap-2 text-[12px]">
					<input
						type="text"
						placeholder="Updates in your inbox..."
						class="w-[200px] rounded-[32px] px-3 text-bright-red"
					/>
					<button class="bg-bright-red shadow-br text-white rounded-[32px]">Go</button>
				</div>
				<p class="text-dark-grayish-blue text-[13px]">
					Copyright 2023. All Rights Reserved
				</p>
			</article>
		</div>
	</section>
</template>

<style lang="scss" scoped>
	a:hover {
		color: hsl(12 88% 59%);
	}
	a img:hover {
		color: hsl(12 88% 59%);
	}

	button {
		width: 60px;
		margin: 0;
		padding: 11px 20px;
		box-shadow: none;
		font-size: 12px !important;
	}
	@media (max-width: 1920px) {
		section {
			.down-footer {
				padding: 70px 64px;
				.redes {
					gap: 90px;
					div {
						gap: 16px;
					}
					img {
						width: 180px;
					}
					.icon {
						width: 26px;
						height: 26px;
					}
				}
				.flex-links {
					gap: 280px;
					.links {
						gap: 13px;
					}
				}
				.copy {
					gap: 86px;

					div {
						font-size: 14px;
					}
				}
			}
		}
	}
	@media (max-width: 1440px) {
		section {
			.down-footer {
				padding: 66px 64px;
				.redes {
					div {
						gap: 14px;
					}
					img {
						width: 156px;
					}
					.icon {
						width: 22px;
						height: 22px;
					}
				}
				.flex-links {
					gap: 230px;
					.links {
						gap: 15px;
					}
				}
				.copy {
					gap: 82px;
				}
			}
		}
	}
	@media (max-width: 1366px) {
		section {
			.down-footer {
				padding: 60px 64px;
				.redes {
					gap: 84px;
					div {
						gap: 14px;
					}
					img {
						width: 150px;
					}
					.icon {
						width: 20px;
						height: 20px;
					}
				}
				.flex-links {
					gap: 210px;
					.links {
						gap: 15px;
					}
				}
				.copy {
					gap: 72px;
				}
			}
		}
	}
	@media (max-width: 1280px) {
		section {
			.down-footer {
				padding: 56px 64px;
				.redes {
					gap: 80px;
					div {
						gap: 12px;
					}
					img {
						width: 144px;
					}
					.icon {
						width: 20px;
						height: 20px;
					}
				}
				.flex-links {
					gap: 190px;
					.links {
						gap: 15px;
					}
				}
				.copy {
					gap: 67px;
				}
			}
		}
	}
	@media (max-width: 420px) {
		section {
			.down-footer {
				flex-direction: column-reverse;
				align-items: center;
				padding: 45px 20px 30px 20px;
				margin: 0 auto;
				gap: 40px;
				.redes {
					flex-direction: column-reverse;
					align-items: center;
					gap: 40px;
					p {
						display: block;
						font-size: 11px;
					}
					div {
						gap: 32px;
					}
					img {
						width: 144px;
					}
					.icon {
						width: 33px;
						height: 33px;
					}
				}
				.flex-links {
					gap: 100px;
					font-size: 12px;
					.links {
						gap: 15px;
					}
				}
				.copy {
					p {
						display: none;
					}
					input {
						width: 250px;
						height: 44px;
					}
					button {
						width: 70px;
						height: 44px;
						text-transform: uppercase;
					}
				}
			}
		}
	}
</style>
