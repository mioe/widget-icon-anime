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

		<svg
			class="WidgetCssAnimationWaCircle"
			viewBox="0 0 148 148"
			fill="none"
			xmlns="http://www.w3.org/2000/svg"
		>
			<path
				class="path"
				fill-rule="evenodd"
				clip-rule="evenodd"
				d="M126.437 21.5065C119.596 14.6618 111.468 9.2378 102.522 5.54686C93.5757 1.85592 83.9879 -0.0290926 74.3103 0.000339407C33.6963 0.000339407 0.634284 32.8972 0.617766 73.3394C0.599799 86.2171 3.99432 98.8696 10.4558 110.009L0 148L39.0646 137.802C49.8779 143.66 61.9825 146.726 74.2806 146.721H74.3103C114.921 146.721 147.98 113.821 148 73.3824C148.024 63.7378 146.131 54.1847 142.429 45.2788C138.727 36.3729 133.291 28.2921 126.437 21.5065ZM74.3103 134.343H74.2839C63.3206 134.346 52.5567 131.412 43.1115 125.846L40.875 124.525L17.6939 130.577L23.8815 108.083L22.4246 105.771C16.2944 96.0652 13.0466 84.8186 13.059 73.3394C13.059 39.7323 40.5479 12.3887 74.3335 12.3887C90.5407 12.3598 106.096 18.7696 117.577 30.2085C129.059 41.6474 135.527 57.1784 135.558 73.3857C135.545 106.996 108.069 134.343 74.3103 134.343Z"
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
	width: 280px;
	position: relative;
	display: flex;
	aspect-ratio: 1 / 1;
	border-radius: 50%;
	background-color: red;
	color: yellow;
	/* transform: scale(0.2); */
}


@keyframes dash {
  from {
    stroke-dashoffset: 822;
  }
  to {
    stroke-dashoffset: 0;
  }
}

.path {
  stroke-dasharray: 1000;
  stroke-dashoffset: 1000;
  animation: dash 5s linear alternate infinite;
}

.WidgetCssAnimationWaCircle {
	all: unset;
	display: flex;
	position: absolute;
	top: 54px;
	left: 54px;
	width: 170px;
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
		transform: translate(30px, -5px) rotate(-20deg) scale(0.9);
		opacity: 1;
	}

	22.4% {
		transform: translate(45px, -13px) rotate(-33deg) scale(0.85);
		opacity: 1;
	}

	22.8% {
		transform: translate(56px, -26px) rotate(-45deg) scale(0.76);
		opacity: 1;
	}

	23.6% {
		transform: translate(51px, -53px) rotate(-74deg) scale(0.63);
		opacity: 1;
	}

	24% {
		transform: translate(41px, -61px) rotate(-89deg) scale(0.55);
		opacity: 1;
	}

	24.4% {
		transform: translate(29px, -64px) rotate(-103deg) scale(0.5);
		opacity: 1;
	}

	24.8% {
		transform: translate(13px, -67px) rotate(-119deg) scale(0.4);
		opacity: 1;
	}

	25.6% {
		transform: translate(-14px, -63px) rotate(-144deg) scale(0.29);
		opacity: 1;
	}

	26.8% {
		transform: translate(-42px, -49px) rotate(-170deg) scale(0.16);
		opacity: 1;
	}

	28% {
		transform: translate(-53px, -37px) rotate(-181deg) scale(0.09);
		opacity: 1;
	}

	29% {
		transform: translate(-53px, -37px) rotate(-181deg) scale(0.09);
		opacity: 0;
	}

	30% {
		transform: translate(-53px, -37px) rotate(-181deg) scale(0.08);
		opacity: 0;
	}

	82.4% {
		transform: translate(20px, -85px) rotate(-130deg) scale(0.08);
		opacity: 0;
	}

	83.6% {
		transform: translate(2px, -83px) rotate(-144deg) scale(0.09);
		opacity: 1;
	}

	84% {
		transform: translate(-10px, -79px) rotate(-151deg) scale(0.09);
		opacity: 1;
	}

	84.8% {
		transform: translate(-44px, -64px) rotate(-182deg) scale(0.1);
		opacity: 1;
	}

	85.2% {
		transform: translate(-60px, -49px) rotate(-203deg) scale(0.13);
		opacity: 1;
	}

	85.6% {
		transform: translate(-71px, -32px) rotate(-230deg) scale(0.18);
		opacity: 1;
	}

	86% {
		transform: translate(-75px, -11px) rotate(-253deg) scale(0.25);
		opacity: 1;
	}

	86.4% {
		transform: translate(-71px, 7px) rotate(-281deg) scale(0.35);
		opacity: 1;
	}

	86.8% {
		transform: translate(-61px, 21px) rotate(-307deg) scale(0.45);
		opacity: 1;
	}

	87.2% {
		transform: translate(-47px, 26px) rotate(-324deg) scale(0.55);
		opacity: 1;
	}

	87.6% {
		transform: translate(-33px, 25px) rotate(-334deg) scale(0.63);
		opacity: 1;
	}

	88% {
		transform: translate(-24px, 20px) rotate(-341deg) scale(0.72);
		opacity: 1;
	}

	88.4% {
		transform: translate(-16px, 16px) rotate(-346deg) scale(0.8);
		opacity: 1;
	}

	88.4% {
		transform: translate(-16px, 16px) rotate(-346deg) scale(0.8);
		opacity: 1;
	}

	88.8% {
		transform: translate(-10px, 9px) rotate(-350deg) scale(0.88);
		opacity: 1;
	}

	89.6% {
		transform: translate(-3px, 4px) rotate(-357deg) scale(0.95);
		opacity: 1;
	}

	91.2% {
		transform: translate(0px, 0px) rotate(-360deg) scale(1);
		opacity: 1;
	}

	to {
		transform: translate(0px, 0px) rotate(-360deg) scale(1);
		opacity: 1;
	}
}

.WidgetCssAnimationTgMessage {
	all: unset;
	display: flex;
	position: absolute;
	top: 79px;
	left: 37px;
	width: 171px;
	height: 141px;
	opacity: 0;

	/* animation-duration: 10s;
	animation-name: slidein;
	animation-iteration-count: infinite;
	animation-timing-function: linear; */
}
</style>
