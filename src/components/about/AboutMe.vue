<script>
export default {
	setup() {
		return {
			bios: [
				{
					id: 1,
					bio:
						'Hello, I am a Front-end Developer with three years of experience working with technologies such as Javascript, Vue, React and Typescript. I have a strong commitment to code quality and am always seeking to learn and stay up to date with the latest technology trends.',
				},
				{
					id: 2,
					bio:
						'I am results-oriented, with skills in teamwork, problem-solving, and resilience. I am very interested in collaborating on challenging projects with high-performance teams. Additionally, I have a proactive profile that seeks to understand user needs and create solutions that exceed their expectations.',
				},
				{
					id: 2,
					bio:
						'If you would like to see my projects, I invite you to visit my profile on Github, where some of the projects I have developed are available: https://github.com/guilherme-studier.',
				},
				{
					id: 2,
					bio:
						'Thank you for your attention, and I look forward to contributing to the success of your company.',
				},
			],
		};
	},
};
</script>

<template>
	<div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
		<!-- About profile image -->
		<div class="w-full sm:w-1/4 mb-7 sm:mb-0">
			<img
				src="@/assets/images/profile.jpeg"
				class="rounded-xl w-96"
				alt=""
			/>
		</div>

		<!-- About details -->
		<div class="w-full sm:w-3/4 text-left">
			<p
				v-for="bio in bios"
				:key="bio.id"
				class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
			>
				{{ bio.bio }}
			</p>
		</div>
	</div>
</template>
