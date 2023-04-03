<script setup lang="ts">
import { ref } from 'vue'
const n = ref(1)
const opacity = ref(0.5)
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
	</header>

	<div
		class="absolute"
		:style="{
			opacity
		}"
	>
		<img
			:src="`/images/p${n}.png`"
			alt=""
			class="w-[304px]"
		>
	</div>
</template>
