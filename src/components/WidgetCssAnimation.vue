<script setup lang="ts">
import { ref } from 'vue'
const opacity = ref(0.5)
</script>

<template>
	<div
		class="WidgetCssAnimation"
		:style="{
			opacity
		}"
	>
		<svg
			class="WidgetCssAnimationTgMessage"
			viewBox="0 0 143 118"
			fill="none"
			xmlns="http://www.w3.org/2000/svg"
		>
			<path
				d="M9.82908 50.7988C48.2226 34.1478 73.8183 23.1694 86.6161 17.8656C123.199 2.72029 130.791 0.0898904 135.75 0.000776466C136.84 -0.0166366 139.268 0.251727 140.853 1.52698C142.169 2.60249 142.54 4.057 142.725 5.07822C142.89 6.09842 143.116 8.42358 142.931 10.2386C140.955 30.9704 132.376 81.2799 128.014 104.501C126.182 114.326 122.541 117.62 119.022 117.942C111.368 118.642 105.566 112.91 98.1588 108.078C86.5749 100.512 80.032 95.8044 68.7773 88.4233C55.7737 79.893 64.2096 75.2037 71.6167 67.542C73.5508 65.5364 107.253 35.0225 107.891 32.2549C107.973 31.9087 108.056 30.6181 107.274 29.9379C106.512 29.2557 105.381 29.4893 104.558 29.6737C103.385 29.9359 84.8878 42.1209 49.0044 66.2268C43.7577 69.82 39.0048 71.5715 34.7252 71.4794C30.034 71.379 20.9809 68.8326 14.2528 66.657C6.02265 63.9877 -0.540875 62.5762 0.0352334 58.0426C0.323288 55.6826 3.59476 53.2674 9.82908 50.7988Z"
				fill="currentColor"
			/>
		</svg>
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

<style>
:root {
	--widget-scale: 1;
}

.WidgetCssAnimation {
	all: unset;
	width: calc(280px * var(--widget-scale));
	position: relative;
	display: flex;
	aspect-ratio: 1 / 1;
	border-radius: 50%;
	background-color: red;
	color: yellow;
}

@keyframes slidein {
	from {
		transform: translate(0, 0) rotate(0) scale(1);
		opacity: 1;
	}

	20% {
		transform: translate(0, 0) rotate(0) scale(1);
		opacity: 1;
	}

	22% {
		transform: translate(calc(30px * var(--widget-scale)), calc(-5px * var(--widget-scale))) rotate(-20deg) scale(0.9);
		opacity: 1;
	}

	22.4% {
		transform: translate(calc(45px * var(--widget-scale)), calc(-13px * var(--widget-scale))) rotate(-33deg) scale(0.85);
		opacity: 1;
	}

	22.8% {
		transform: translate(calc(56px * var(--widget-scale)), calc(-26px * var(--widget-scale))) rotate(-45deg) scale(0.76);
		opacity: 1;
	}

	23.6% {
		transform: translate(calc(51px * var(--widget-scale)), calc(-53px * var(--widget-scale))) rotate(-74deg) scale(0.63);
		opacity: 1;
	}

	24% {
		transform: translate(calc(41px * var(--widget-scale)), calc(-61px * var(--widget-scale))) rotate(-89deg) scale(0.55);
		opacity: 1;
	}

	24.4% {
		transform: translate(calc(29px * var(--widget-scale)), calc(-64px * var(--widget-scale))) rotate(-103deg) scale(0.5);
		opacity: 1;
	}

	24.8% {
		transform: translate(calc(13px * var(--widget-scale)), calc(-67px * var(--widget-scale))) rotate(-119deg) scale(0.4);
		opacity: 1;
	}

	25.6% {
		transform: translate(calc(-14px * var(--widget-scale)), calc(-63px * var(--widget-scale))) rotate(-144deg) scale(0.29);
		opacity: 1;
	}

	26.8% {
		transform: translate(calc(-42px * var(--widget-scale)), calc(-49px * var(--widget-scale))) rotate(-170deg) scale(0.16);
		opacity: 1;
	}

	28% {
		transform: translate(calc(-53px * var(--widget-scale)), calc(-37px * var(--widget-scale))) rotate(-181deg) scale(0.09);
		opacity: 1;
	}

	29% {
		transform: translate(calc(-53px * var(--widget-scale)), calc(-37px * var(--widget-scale))) rotate(-181deg) scale(0.09);
		opacity: 0;
	}

	30% {
		transform: translate(calc(-53px * var(--widget-scale)), calc(-37px * var(--widget-scale))) rotate(-181deg) scale(0.08);
		opacity: 0;
	}

	82.4% {
		transform: translate(calc(20px * var(--widget-scale)), calc(-85px * var(--widget-scale))) rotate(-130deg) scale(0.08);
		opacity: 1;
	}

	83.6% {
		transform: translate(calc(2px * var(--widget-scale)), calc(-83px * var(--widget-scale))) rotate(-144deg) scale(0.09);
		opacity: 1;
	}

	84% {
		transform: translate(calc(-10px * var(--widget-scale)), calc(-79px * var(--widget-scale))) rotate(-151deg) scale(0.09);
		opacity: 1;
	}

	84.8% {
		transform: translate(calc(-44px * var(--widget-scale)), calc(-64px * var(--widget-scale))) rotate(-182deg) scale(0.1);
		opacity: 1;
	}

	85.2% {
		transform: translate(calc(-60px * var(--widget-scale)), calc(-49px * var(--widget-scale))) rotate(-203deg) scale(0.13);
		opacity: 1;
	}

	85.6% {
		transform: translate(calc(-71px * var(--widget-scale)), calc(-32px * var(--widget-scale))) rotate(-230deg) scale(0.18);
		opacity: 1;
	}

	86% {
		transform: translate(calc(-75px * var(--widget-scale)), calc(-11px * var(--widget-scale))) rotate(-253deg) scale(0.25);
		opacity: 1;
	}

	86.4% {
		transform: translate(calc(-71px * var(--widget-scale)), calc(7px * var(--widget-scale))) rotate(-281deg) scale(0.35);
		opacity: 1;
	}

	86.8% {
		transform: translate(calc(-61px * var(--widget-scale)), calc(21px * var(--widget-scale))) rotate(-307deg) scale(0.45);
		opacity: 1;
	}

	87.2% {
		transform: translate(calc(-47px * var(--widget-scale)), calc(26px * var(--widget-scale))) rotate(-324deg) scale(0.55);
		opacity: 1;
	}

	87.2% {
		transform: translate(calc(-47px * var(--widget-scale)), calc(26px * var(--widget-scale))) rotate(-324deg) scale(0.55);
		opacity: 1;
	}

	to {
		transform: translate(17px, 26px) rotate(0) scale(1);
		opacity: 1;
	}
}

.WidgetCssAnimationTgMessage {
	all: unset;
	display: flex;
	position: absolute;
	top: calc(79px * var(--widget-scale));
	left: calc(37px * var(--widget-scale));
	width: calc(171px * var(--widget-scale));
	height: calc(141px * var(--widget-scale));

		/* animation-duration: 10s;
		animation-name: slidein;
		animation-iteration-count: infinite;
		animation-timing-function: linear; */
}
</style>
