<script>
export default {
	props: ['projectImages'],
};
</script>

<template>
	<div class="grid grid-cols-1 sm:grid-cols-3 sm:gap-10 mt-12">
		<div
			class="mb-10 sm:mb-0"
			v-for="projectImage in projectImages"
			:key="projectImage.id"
		>
			<img
				:src="projectImage.img"
				:class="['rounded-xl', 'cursor-pointer', 'shadow-lg', 'sm:shadow-none']"
				:alt="projectImage.title"
				:style="{ width: '100%', height: '100%' }"
			/>
		</div>
	</div>
</template>
In the updated code, the :style binding is used to apply the width: 100% and height: 100% styles to the <img> tag. The :style attribute accepts an object where you can specify CSS properties and their values.

Make sure to include the class binding `:class="['rounded-xl', 'cursor



