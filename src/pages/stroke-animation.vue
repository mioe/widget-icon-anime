<script setup lang="ts">
import { onMounted } from 'vue'

onMounted(() => {
	const path = document.querySelector('.path')
	// @ts-ignore
	const length = path?.getTotalLength()
	console.log('🦕 length', length)
})
</script>

<template>
	<div class="flex gap-[32px]">
		<svg
			width="148"
			height="148"
			viewBox="0 0 148 148"
			fill="none"
			xmlns="http://www.w3.org/2000/svg"
		>
			<path
				class="path"
				d="
					M 122.194 25.7482
					L 122.205 25.7593
					L 122.216 25.7704
					C 128.504 31.9962 133.492 39.4104 136.888 47.5817
					C 140.285 55.753 142.022 64.5181 142 73.3671
					L 142 73.3795
					C 141.982 110.482 111.633 140.722 74.3104 140.722
					H 74.2807
					H 74.2786C62.9793 140.725 51.8577 137.909 41.9227 132.526
					L 39.8405 131.398
					L 37.5491 131.996
					L 8.54357 139.569
					L 16.2407 111.601
					L 16.9084 109.175
					L 15.6458 106.998
					C 9.71635 96.7762 6.60127 85.1653 6.61776 73.3478
					L 6.61777 73.3419C6.63292 36.2376 36.9839 6.00034 74.3104 6.00034
					H 74.3195L74.3287 6.00031
					C 83.215 5.97329 92.019 7.70418 100.234 11.0934
					C 108.448 14.4825 115.912 19.463 122.194 25.7482 Z"
				stroke="black"
				stroke-width="12"
			/>
		</svg>
		<svg
			width="148"
			height="148"
			viewBox="0 0 148 148"
			fill="none"
			xmlns="http://www.w3.org/2000/svg"
		>
			<path
				class="path"
				d="
					M 6.61776 73.3479
					L 6.61777 73.3419
					C 6.62418 57.6475 12.0481 43.1969 21.1396 31.727
					C 33.5591 16.0586 52.7807 6.00037 74.3104 6.00037
					C 111.637 6.00037 142.018 36.2826 142 73.3795
					C 141.982 110.482 111.633 140.722 74.3104 140.722
					H 74.2807
					H 74.2786
					C 62.9793 140.725 51.8577 137.909 41.9227 132.526
					L 39.8405 131.398L37.5491 131.997
					L 8.54356 139.569L16.2407 111.601
					L 16.9084 109.175
					L 15.6458 106.999
					C 9.71635 96.7762 6.60127 85.1654 6.61776 73.3479 Z
				"
				stroke="black"
				stroke-width="12"
			/>
		</svg>
	</div>
</template>

<style>
.path {
	stroke-dasharray: 456;
	stroke-dashoffset: 0;
	animation: dash 5s linear infinite;
}

@keyframes dash {
	from {
		stroke-dashoffset: 456;
	}
	to {
		stroke-dashoffset: 0;
	}
}
</style>
