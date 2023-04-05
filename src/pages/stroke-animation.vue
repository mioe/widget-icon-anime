<script setup lang="ts">
import { onMounted } from 'vue'

onMounted(() => {
	const path = document.querySelector('.path')
	const length = path?.getTotalLength()
	console.log('🦕 length', length)
})
</script>

<template>
	<div>
		<svg
			width="148"
			height="148"
			viewBox="0 0 148 148"
			fill="none"
			xmlns="http://www.w3.org/2000/svg"
		>
			<path
				class="path"
				d="M122.194 25.7482L122.205 25.7593L122.216 25.7704C128.504 31.9962 133.492 39.4104 136.888 47.5817C140.285 55.753 142.022 64.5181 142 73.3671L142 73.3795C141.982 110.482 111.633 140.722 74.3104 140.722H74.2807H74.2786C62.9793 140.725 51.8577 137.909 41.9227 132.526L39.8405 131.398L37.5491 131.996L8.54357 139.569L16.2407 111.601L16.9084 109.175L15.6458 106.998C9.71635 96.7762 6.60127 85.1653 6.61776 73.3478L6.61777 73.3419C6.63292 36.2376 36.9839 6.00034 74.3104 6.00034H74.3195L74.3287 6.00031C83.215 5.97329 92.019 7.70418 100.234 11.0934C108.448 14.4825 115.912 19.463 122.194 25.7482Z"
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
	animation: dash 5s linear;
}

@keyframes dash {
	from {
		stroke-dashoffset: 0;
	}
	to {
		stroke-dashoffset: 456;
	}
}
</style>
