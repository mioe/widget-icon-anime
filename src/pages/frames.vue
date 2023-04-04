<script setup lang="ts">
import { ref } from 'vue'
import WidgetCssAnimation from '~/components/WidgetCssAnimation.vue'
import WidgetFrames from '~/components/WidgetFrames.vue'

const opacity = ref(0.5)
</script>

<template>
	<div class="min-h-screen flex justify-center items-center">
		<WidgetFrames />
		<WidgetCssAnimation :opacity="opacity" />
	</div>

	<footer class="fixed bottom-[24px] left-[50%] transform -translate-x-[50%]">
		<input
			v-model="opacity"
			type="range"
			step="0.1"
			min="0"
			max="1"
		>
	</footer>
</template>
