<script setup lang="ts">
import Pfp from "@/components/Pfp.vue";
import LogoContainer from "@/components/logo/LogoContainer.vue";
import Desc from "@/components/Desc.vue";
import Links from "@/components/Links.vue";

import YoruJapaneseText from "@/designs/bg/YoruJapaneseText.vue";
import YoruDesc from "@/designs/bg/YoruDesc.vue";
import ColumnOfEllipses from "@/designs/bg/ColumnOfEllipses.vue";

import TopLeftSquares from "@/designs/content/TopLeftSquares.vue";
import BunchaLines from "@/designs/content/BunchaLines.vue";
import TopRightCornerOutline from "@/designs/content/TopRightCornerOutline.vue";
import BottomRightDottedQuarterEllipse from "@/designs/content/BottomRightDottedQuarterEllipse.vue";

import ValoBg from "@/components/ValoBg.vue";
import GrainOverlay from "@/components/GrainOverlay.vue";

// =============================

/*import { onMounted } from "vue";

let app: HTMLElement | null = null;

onMounted(() => {
	app = document.getElementById("app")

	window.onmousemove = (e) => {
		if (!app) return;

		const { clientX, clientY } = e;
		const windowWidthHalf = window.innerWidth / 2;
		const windowHeightHalf = window.innerHeight / 2;

		const fromCenterX = (clientX - windowWidthHalf) / windowWidthHalf;
		const fromCenterY = (clientY - windowHeightHalf) / windowHeightHalf;

		const maxTranslate = 1
		const translateX = `${fromCenterX * maxTranslate}rem`
		const translateY = `${fromCenterY  * maxTranslate}rem`

		app.style.setProperty("--dot-grid-translate-x", translateX)
		app.style.setProperty("--dot-grid-translate-y", translateY)
	};
});*/
</script>

<template>
	<ValoBg />

	<div
		class="drop-shadow-night-light/25 lg:rows-[auto_auto] relative isolate grid w-[34.75em] grid-cols-[61%_auto] gap-[1.25em] text-[min(2vw,_1rem)] drop-shadow-[0_0_0.25em] lg:w-[54.375em] lg:grid-cols-[33.33%_min-content_auto] lg:gap-0 lg:text-base"
	>
		<Pfp />
		<LogoContainer />
		<Links />
		<Desc />

		<TopLeftSquares />
		<BunchaLines />
		<TopRightCornerOutline />
		<BottomRightDottedQuarterEllipse />
	</div>

	<YoruJapaneseText />
	<YoruDesc />
	<ColumnOfEllipses />

	<GrainOverlay />
</template>

<style>
@reference "@/assets/main.css";

.logo-container,
.links {
	@apply lg:ml-[1.25em];
}
</style>
