<script setup lang="ts">
defineProps({
	opacity: {
		type: Number,
		default: 1,
	},
	isActive: {
		type: Boolean,
		default: false,
	},
})
</script>

<template>
	<div
		class="WidgetCssAnimation"
		:class="isActive && 'is-active'"
		:style="{
			opacity,
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
			width="148"
			height="148"
			viewBox="0 0 148 148"
			fill="none"
			xmlns="http://www.w3.org/2000/svg"
		>
			<path
				class="WidgetCssAnimationWaCirclePathIn"
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
				stroke="currentColor"
				stroke-width="12"
			/>
		</svg>

		<svg
			class="WidgetCssAnimationWaCircle"
			width="148"
			height="148"
			viewBox="0 0 148 148"
			fill="none"
			xmlns="http://www.w3.org/2000/svg"
		>
			<path
				class="WidgetCssAnimationWaCirclePathOut"
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
				stroke="currentColor"
				stroke-width="12"
			/>
		</svg>

		<svg
			class="WidgetCssAnimationWaPhone"
			width="75"
			height="70"
			viewBox="0 0 75 70"
			fill="none"
			xmlns="http://www.w3.org/2000/svg"
		>
			<path
				d="M71.0471 49.2315C69.2069 48.313 60.1442 43.8791 58.4659 43.2679C56.7875 42.6567 55.5485 42.3494 54.3228 44.1864C53.097 46.0234 49.5651 50.1334 48.4914 51.3724C47.4176 52.6113 46.3438 52.7468 44.5036 51.8283C42.6633 50.9098 36.7262 48.977 29.6922 42.7327C24.2176 37.8726 20.5238 31.8727 19.4501 30.0391C18.3763 28.2054 19.3344 27.2109 20.2562 26.2991C21.0855 25.4764 22.0965 24.1581 23.0183 23.0877C23.9401 22.0172 24.2473 21.2507 24.8586 20.0283C25.4698 18.8058 25.1658 17.7353 24.7066 16.8202C24.2473 15.905 20.5635 6.88202 19.0305 3.21139C17.5338 -0.363436 16.0173 0.122243 14.8874 0.066077C13.8136 0.0132146 12.5747 0 11.3555 0C10.4235 0.0242596 9.50653 0.240389 8.6618 0.634898C7.81708 1.02941 7.06275 1.59382 6.44592 2.2929C4.75762 4.12987 0 8.57032 0 17.5834C0 26.5964 6.60781 35.3187 7.51969 36.5412C8.43156 37.7636 20.504 56.2754 38.9761 64.2146C42.4062 65.6836 45.911 66.9717 49.4759 68.0736C53.8867 69.4679 57.9009 69.2729 61.0726 68.8005C64.6111 68.2751 71.9755 64.3666 73.5052 60.0848C75.0349 55.8029 75.0382 52.1356 74.579 51.3724C74.1198 50.6092 72.8907 50.1466 71.0471 49.2315Z"
				fill="currentColor"
			/>
		</svg>
	</div>
</template>

<style>
.WidgetCssAnimation {
	all: unset;
	width: 280px;
	position: relative;
	display: flex;
	aspect-ratio: 1 / 1;
	border-radius: 50%;
	background-color: red;
	color: yellow;
}

.WidgetCssAnimation.is-active {
	background-color: #0088cc;
	color: white;
	animation-duration: 10s;
	animation-name: WidgetCssColorAnimation;
	animation-iteration-count: infinite;
	animation-timing-function: ease-in-out;
}

@keyframes WidgetCssColorAnimation {
	from {
		background-color: #0088cc;
	}

	22% {
		background-color: #0088cc;
	}

	28.8% {
		background-color: #25d366;
	}

	82% {
		background-color: #25d366;
	}

	88% {
		background-color: #0088cc;
	}

	to {
		background-color: #0088cc;
	}
}

.WidgetCssAnimationWaPhone {
	position: absolute;
	top: 107px;
	left: 101px;
	transform: scale(1.15);
	transform-origin: center center;
}

.WidgetCssAnimation.is-active .WidgetCssAnimationWaPhone {
	animation-duration: 10s;
	animation-name: WidgetCssAnimationWaPhoneAnimation;
	animation-iteration-count: infinite;
	animation-timing-function: ease-in-out;
}

@keyframes WidgetCssAnimationWaPhoneAnimation {
	from {
		transform: scale(0);
		opacity: 0;
	}

	34% {
		transform: scale(0);
		opacity: 0;
	}

	34.01% {
		transform: scale(0);
		opacity: 1;
	}

	38% {
		transform: scale(1.24);
		opacity: 1;
	}

	41.2% {
		transform: scale(1.15);
		opacity: 1;
	}

	78.8% {
		transform: scale(1.15);
		opacity: 1;
	}

	81.2% {
		transform: scale(1.3);
		opacity: 1;
	}

	83.6% {
		transform: scale(0);
		opacity: 1;
	}

	83.601% {
		transform: scale(0);
		opacity: 0;
	}

	to {
		transform: scale(0);
		opacity: 0;
	}
}

.WidgetCssAnimationWaCircle {
	position: absolute;
	top: 66px;
	left: 67px;
	transform: scale(1.15);
}

.WidgetCssAnimation.is-active .WidgetCssAnimationWaCirclePathIn {
	stroke-dashoffset: 912;
	stroke-dasharray: 456;
	animation-duration: 10s;
	animation-name: WidgetCssAnimationWaCirclePathInAnimation;
	animation-iteration-count: infinite;
	animation-timing-function: ease-in-out;
}

.WidgetCssAnimation.is-active .WidgetCssAnimationWaCirclePathOut {
	stroke-dashoffset: 456;
	stroke-dasharray: 456;
	animation-duration: 10s;
	animation-name: WidgetCssAnimationWaCirclePathOutAnimation;
	animation-iteration-count: infinite;
	animation-timing-function: ease-in-out;
}

@keyframes WidgetCssAnimationWaCirclePathOutAnimation {
	from {
		stroke-dashoffset: 0;
		opacity: 0;
	}

	40.8% {
		stroke-dashoffset: 0;
		opacity: 0;
	}

	40.801% {
		stroke-dashoffset: 0;
		opacity: 1;
	}

	70.8% {
		stroke-dashoffset: 0;
		opacity: 1;
	}

	82% {
		stroke-dashoffset: 456;
		opacity: 1;
	}

	82.01% {
		stroke-dashoffset: 456;
		opacity: 0;
	}

	to {
		stroke-dashoffset: 456;
		opacity: 0;
	}
}

@keyframes WidgetCssAnimationWaCirclePathInAnimation {
	from {
		stroke-dashoffset: 456;
		opacity: 0;
	}

	28.8% {
		stroke-dashoffset: 456;
		opacity: 0;
	}

	28.801% {
		stroke-dashoffset: 456;
		opacity: 1;
	}

	41% {
		stroke-dashoffset: 0;
		opacity: 1;
	}

	41.001% {
		stroke-dashoffset: 0;
		opacity: 0;
	}

	to {
		stroke-dashoffset: 0;
		opacity: 0;
	}
}

@keyframes WidgetCssAnimationTgMessageAnimation {
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

.WidgetCssAnimation.is-active .WidgetCssAnimationTgMessage {
	animation-duration: 10s;
	animation-name: WidgetCssAnimationTgMessageAnimation;
	animation-iteration-count: infinite;
	animation-timing-function: linear;
}

.WidgetCssAnimationTgMessage {
	all: unset;
	display: flex;
	position: absolute;
	top: 79px;
	left: 37px;
	width: 171px;
	height: 141px;
}
</style>
