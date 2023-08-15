<script>
	import { defineComponent } from 'vue';
	import { Carousel, Slide, Pagination } from 'vue3-carousel';
	import 'vue3-carousel/dist/carousel.css';

	export default defineComponent({
		name: 'WrapAround',
		components: {
			Carousel,
			Slide,
			Pagination,
		},
		data() {
			return {
				slides: [
					{
						id: 1,
						image: '/avatar-anisha.png',
						name: 'Anisha Li',
						msg: '“Manage has supercharged our team’s workflow. The ability to maintain visibility on larger milestones at all times keeps everyone motivated.”',
					},
					{
						id: 2,
						image: '/avatar-ali.png',
						name: 'Ali Bravo',
						msg: '“We have been able to cancel so many other subscriptions since using Manage. There is no more cross-channel confusion and everyone is much more focused.”',
					},
					{
						id: 3,
						image: '/avatar-richard.png',
						name: 'Richard Watts',
						msg: '“Manage allows us to provide structure and process. It keeps us organized and focused. I can’t stop recommending them to everyone I talk to!”',
					},
					{
						id: 4,
						image: '/avatar-shanai.png',
						name: 'Shanai Gough',
						msg: '“Their software allows us to track, manage and collaborate on our projects from anywhere. It keeps the whole team in-sync without being intrusive.”',
					},
				],
			};
		},
	});
</script>

<template>
	<section class="flex flex-col items-center mb-32">
		<h2 class="text-4xl text-dark-blue font-semibold text-center mb-20">
			What they’ve said
		</h2>
		<Carousel :items-to-show="2.6" :autoplay="4000" :wrap-around="true" class="carousel">
			<Slide v-for="{ id, image, name, msg } in slides" :key="id">
				<div class="carousel__item relative mr-6 testimonial-card bg-very-light-gray">
					<img
						:src="image"
						class="w-[60px] h-[60px] rounded-full -mt-14 mx-auto mb-5 z-10"
					/>
					<h4 class="font-semibold mb-4">{{ name }}</h4>
					<p class="text-dark-grayish-blue">
						{{ msg }}
					</p>
				</div>
			</Slide>

			<template #addons>
				<div class="hidden">
					<Pagination />
				</div>
			</template>
		</Carousel>
		<button class="bg-bright-red shadow-br text-white rounded-[32px] mt-10">
			Get Started
		</button>
	</section>
</template>

<style lang="scss" scoped>
	.testimonial-card {
		margin-top: 30px;
		padding: 30px;
	}
	@media (max-width: 420px) {
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
