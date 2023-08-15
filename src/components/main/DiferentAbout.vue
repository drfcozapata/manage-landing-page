<template>
	<div class="flex gap-[95px] mb-32 diferent-about">
		<section class="flex flex-col gap-8 w-1/2 about-left">
			<h2 class="text-4xl text-dark-blue font-semibold">
				What’s different about Manage?
			</h2>
			<p class="text-dark-grayish-blue mr-[200px]">
				Manage provides all the functionality your team needs, without the complexity. Our
				software is tailor-made for modern digital product teams.
			</p>
		</section>
		<section class="flex flex-col gap-12 w-1/2 about-right">
			<article class="flex gap-7">
				<div
					class="-mt-2 h-9 py-[6px] px-5 rounded-3xl bg-bright-red text-white font-semibold number"
				>
					01
				</div>
				<div>
					<h3 class="font-semibold mb-5">Track company-wide progress</h3>
					<p class="text-dark-grayish-blue description">
						See how your day-to-day tasks fit into the wider vision. Go from tracking
						progress at the milestone level all the way done to the smallest of details.
						Never lose sight of the bigger picture again.
					</p>
				</div>
			</article>
			<article class="flex gap-7">
				<div
					class="-mt-2 h-9 py-[6px] px-5 rounded-3xl bg-bright-red text-white font-semibold number"
				>
					02
				</div>
				<div>
					<h3 class="font-semibold mb-5">Advanced built-in reports</h3>
					<p class="text-dark-grayish-blue description">
						Set internal delivery estimates and track progress toward company goals. Our
						customisable dashboard helps you build out the reports you need to keep key
						stakeholders informed.
					</p>
				</div>
			</article>
			<article class="flex gap-7">
				<div
					class="-mt-2 h-9 py-[6px] px-5 rounded-3xl bg-bright-red text-white font-semibold number"
				>
					03
				</div>
				<div>
					<h3 class="font-semibold mb-5">Everything you need in one place</h3>
					<p class="text-dark-grayish-blue description">
						Stop jumping from one service to another to communicate, store files, track
						tasks and share documents. Manage offers an all-in-one team productivity
						solution.
					</p>
				</div>
			</article>
		</section>
	</div>
</template>

<style lang="scss" scoped>
	@media (max-width: 1920px) {
		.diferent-about {
			gap: 110px;
			margin-bottom: 180px;
			.about-left {
				h2 {
					font-size: 43px;
					line-height: 56px;
				}
				p {
					margin-right: 250px;
				}
			}
			.about-right {
				article {
					gap: 34px;

					.number {
						height: 44px;
						padding: 8px 28px;
					}
				}
			}
		}
	}
	@media (max-width: 1440px) {
		.diferent-about {
			margin-bottom: 160px;
			.about-left {
				h2 {
					font-size: 36px;
					line-height: 40px;
				}
				p {
					margin-right: 190px;
				}
			}
			.about-right {
				article {
					gap: 28px;

					.number {
						height: 36px;
						padding: 6px 20px;
					}
				}
			}
		}
	}
	@media (max-width: 1366px) {
		.diferent-about {
			gap: 105px;
			margin-bottom: 140px;
			.about-left {
				h2 {
					font-size: 36px;
					line-height: 40px;
				}
				p {
					margin-right: 190px;
				}
			}
			.about-right {
				article {
					gap: 30px;

					.number {
						height: 34px;
						padding: 6px 22px;
					}
					p {
						padding-right: 10px;
					}
				}
			}
		}
	}
	@media (max-width: 1280px) {
		.diferent-about {
			margin-bottom: 120px;
			gap: 135px;
			.about-left {
				p {
					margin-right: 210px;
				}
			}
			.about-right {
				article {
					gap: 30px;

					.number {
						height: 34px;
						padding: 6px 22px;
					}
					p {
						padding-right: 15px;
					}
				}
			}
		}
	}
	@media (max-width: 420px) {
		.diferent-about {
			flex-direction: column;
			margin-bottom: 70px;
			gap: 55px;
			.about-left {
				width: 100%;
				text-align: center;
				padding: 0 20px;
				gap: 15px;
				h2 {
					font-size: 30px;
				}
				p {
					font-size: 15px;
					margin-right: 0px;
					line-height: 27px;
				}
			}
			.about-right {
				width: 100%;
				article {
					gap: 15px;
					padding-left: 15px;

					.number {
						height: 32px;
						padding: 6px 22px;
						z-index: 10;
					}
					h3 {
						height: 32px;
						background-color: hsl(13, 100%, 96%);
						margin-top: -8px;
						margin-left: -25px;
						padding-top: 6px;
						padding-left: 25px;
					}
					p {
						padding-right: 15px;
					}
					.description {
						font-size: 14px;
						margin-top: -8px;
						margin-left: -72px;
						padding-right: 15px;
						line-height: 26px;
					}
				}
			}
		}
	}
</style>
