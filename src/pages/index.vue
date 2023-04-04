<script setup lang="ts">
const staticPrefix = import.meta.url[5] === ':'
const staticFiles = [
	{ size: '410 KB', src: '/mixed-logo.gif' },
	{ size: '520 KB', src: '/output-adobe.gif' },
	{ size: '1,9 MB', src: '/output-ffmpeg.gif' },
	{ size: '125 KB', src: '/output-gifski.gif' },
]
</script>

<template>
	<div class="min-h-screen flex flex-col px-[8px]">
		<div>
			<h2>Static files:</h2>
			<div class="flex">
				<div
					v-for="(f, idx) in staticFiles"
					:key="idx"
					class="border p-[8px] flex flex-col gap-[4px]"
				>
					<p>{{ f.src }} <span>{{ f.size }}</span></p>
					<img
						:src="`${staticPrefix ? '/widget-icon-anime' : ''}${f.src}`"
						alt=""
					>
				</div>
			</div>
		</div>
	</div>
</template>
