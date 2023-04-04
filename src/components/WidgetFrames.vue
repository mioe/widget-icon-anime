<script setup lang="ts">
import { ref, computed } from 'vue'
const lastFrame = 250
const n = ref(1)
const opacity = ref(0.5)
const percent = computed(() => (100 * n.value) / lastFrame)
const staticPrefix = import.meta.url[5] === ':'
</script>

<template>
	<header class="fixed top-[24px] left-[50%] transform -translate-x-[50%]">
		<input
			v-model="n"
			type="number"
			min="1"
			max="250"
		>
		<input
			v-model="n"
			type="range"
			min="1"
			max="250"
		>
		<input
			v-model="opacity"
			type="range"
			step="0.1"
			min="0"
			max="1"
		>

		<span>
			{{ percent }}
		</span>
	</header>

	<div
		class="absolute"
		:style="{
			opacity
		}"
	>
		<img
			:src="`${staticPrefix ? '/widget-icon-anime' : ''}/images/p${n}.png`"
			alt=""
			class="w-[304px]"
		>
	</div>
</template>
