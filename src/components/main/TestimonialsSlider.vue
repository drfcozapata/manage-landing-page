<script setup>
	//
</script>

<template>
	<section class="flex flex-col items-center mb-32">
		<h2 class="text-4xl text-dark-blue font-semibold text-center mb-24">
			What they’ve said
		</h2>
		<article class="flex gap-6 -ml-7 mb-11">
			<div class="min-h-48 w-[516px] bg-very-light-gray text-center p-7 testimonial-card">
				<img
					src="/avatar-anisha.png"
					alt=""
					class="w-[60px] h-[60px] rounded-full -mt-14 mx-auto mb-5"
				/>
				<h4 class="font-semibold mb-4">Anisha Li</h4>
				<p class="text-dark-grayish-blue">
					“Manage has supercharged our team’s workflow. The ability to maintain visibility
					on larger milestones at all times keeps everyone motivated.”
				</p>
			</div>
			<div class="min-h-48 w-[516px] bg-very-light-gray text-center p-7 testimonial-card">
				<img
					src="/avatar-ali.png"
					alt=""
					class="w-[60px] h-[60px] rounded-full -mt-14 mx-auto mb-5"
				/>
				<h4 class="font-semibold mb-4">Ali Bravo</h4>
				<p class="text-dark-grayish-blue">
					“We have been able to cancel so many other subscriptions since using Manage.
					There is no more cross-channel confusion and everyone is much more focused.”
				</p>
			</div>
			<div
				class="{min-h-48 w-[516px] bg-very-light-gray text-center p-7 testimonial-card hidden:screen.width <= 375}"
			>
				<img
					src="/avatar-richard.png"
					alt=""
					class="w-[60px] h-[60px] rounded-full -mt-14 mx-auto mb-5"
				/>
				<h4 class="font-semibold mb-4">Richard Watts</h4>
				<p class="text-dark-grayish-blue">
					“Manage allows us to provide structure and process. It keeps us organized and
					focused. I can’t stop recommending them to everyone I talk to!”
				</p>
			</div>
			<div
				class="min-h-48 w-[516px] bg-very-light-gray text-center p-7 testimonial-card hidden"
			>
				<img
					src="/avatar-shanai.png"
					alt=""
					class="w-[60px] h-[60px] rounded-full -mt-14 mx-auto mb-5"
				/>
				<h4 class="font-semibold mb-4">Shanai Gough</h4>
				<p class="text-dark-grayish-blue">
					“Their software allows us to track, manage and collaborate on our projects from
					anywhere. It keeps the whole team in-sync without being intrusive.”
				</p>
			</div>
		</article>
		<button class="bg-bright-red shadow-br text-white rounded-[32px] mr-7">
			Get Started
		</button>
	</section>
</template>

<style lang="scss" scoped>
	@media (max-width: 1920px) {
		section {
			margin-bottom: 200px;
			article {
				gap: 32px;
				.testimonial-card {
					width: 620px;
					padding: 35px;
					img {
						width: 70px;
						height: 70px;
						margin-top: -70px;
						margin-bottom: 30px;
					}
				}
			}
		}
	}
	@media (max-width: 1440px) {
		section {
			margin-bottom: 190px;
			article {
				gap: 28px;
				.testimonial-card {
					min-height: 192px;
					width: 527px;
					padding: 32px;
					img {
						width: 64px;
						height: 64px;
						margin-top: -64px;
						margin-bottom: 26px;
					}
				}
			}
		}
	}
	@media (max-width: 1366px) {
		section {
			margin-bottom: 180px;
			article {
				gap: 24px;
				.testimonial-card {
					min-height: 192px;
					width: 494px;
					padding: 30px;
					img {
						width: 62px;
						height: 62px;
						margin-top: -62px;
						margin-bottom: 24px;
					}
				}
			}
		}
	}
	@media (max-width: 1280px) {
		section {
			margin-bottom: 160px;
			article {
				gap: 24px;
				.testimonial-card {
					min-height: 180px;
					width: 465px;
					padding: 30px;
					img {
						width: 60px;
						height: 60px;
						margin-top: -60px;
						margin-bottom: 23px;
					}
				}
			}
		}
	}
	@media (max-width: 375px) {
		section {
			margin-bottom: 40px;
			h2 {
				font-size: 30px;
				margin-bottom: 85px;
			}
			article {
				gap: 24px;
				.testimonial-card {
					min-height: 200px;
					width: 90vw;
					padding: 20px;
					font-size: 14px;
					line-height: 1.8;
					img {
						width: 60px;
						height: 60px;
						margin-top: -50px;
						margin-bottom: 20px;
					}
				}
			}
			button {
				padding: 11px 20px;
			}
		}
	}
</style>
