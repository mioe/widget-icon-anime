<script setup lang="ts">
import WidgetCssAnimation from '~/components/WidgetCssAnimation.vue'

const staticPrefix = import.meta.url[5] === ':'
const staticFiles = [
	{ size: '410 KB', src: '/mixed-logo.gif' },
	{ size: '520 KB', src: '/output-adobe.gif' },
	{ size: '1,9 MB', src: '/output-ffmpeg.gif' },
	{ size: '125 KB', src: '/output-gifski.gif' },
]
</script>

<template>
	<div class="min-h-screen flex flex-col gap-[16px] px-[8px]">
		<div>
			<h2>Static files:</h2>
			<div class="flex gap-[16px]">
				<div
					v-for="(f, idx) in staticFiles"
					:key="idx"
					class="flex flex-col gap-[4px]"
				>
					<p>{{ f.src }} <span>{{ f.size }}</span></p>
					<img
						:src="`${staticPrefix ? '/widget-icon-anime' : ''}${f.src}`"
						alt=""
					>
				</div>
			</div>
		</div>

		<div>
			<h2>Results diff:</h2>
			<div class="flex gap-[16px]">
				<div class="flex flex-col gap-[4px]">
					<p>old gif</p>
					<div class="w-[86px] h-[86px]">
						<img
							:src="`${staticPrefix ? '/widget-icon-anime' : ''}/mixed-logo.gif`"
							alt=""
						>
					</div>
				</div>
				<div class="flex flex-col gap-[4px]">
					<p>new gif - gifski</p>
					<div class="w-[86px] h-[86px]">
						<img
							:src="`${staticPrefix ? '/widget-icon-anime' : ''}/output-gifski.gif`"
							alt=""
							class="rounded-full"
						>
					</div>
				</div>
				<div class="flex flex-col gap-[4px]">
					<p>html + svg + css</p>
					<div class="w-[86px] h-[86px]">
						<WidgetCssAnimation
							is-active
							style="
								transform: scale(0.307);
								transform-origin: top left;
							"
						/>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>
